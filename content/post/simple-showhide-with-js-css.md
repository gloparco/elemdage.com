+++
title       = "Simple Show/Hide with JS & CSS"
description = "Simple JavaScript & CSS tutorial on how to implement a slide in/out"
date        = "2014-03-05"
+++

![JS Logo](/js.jpg) I am frequently asked by front end developers what the best technique is for showing and hiding a div within a web page.  While this can be accomplished many ways, I will outline the technique that I use most often.  It involves adding and removing a class from the DOM node you are looking to show or hide.  The code shown can be used as a starting point, and can be enhanced once you understand the basics.

Note: if you would like to skip the tutorial and jump right to the code, head on over to [github](https://github.com/gloparco/ShowHide").  If you want to see the code in action, you can try it out [here](http://elemdage.com/ShowHide).  The demo will run on mobile devices as well, but be aware that I haven't bothered removing the [300ms delay](http://updates.html5rocks.com/2013/12/300ms-tap-delay-gone-away).

Now on to the tutorial...

## Step 1: the HTML

First, you will need to set up your tags properly.  We will set up two div's of note: a div that acts as a toggle button, and a toggle-able content area:

<div data-height="220" data-theme-id="8299" data-slug-hash="LcIKJ" data-default-tab="html" data-user="gloparco" class='codepen'><pre><code>&lt;div id=&quot;mainContent&quot; class=&quot;mainContent&quot;&gt;
  &lt;h1&gt;Easy Show/Hide Using CSS&lt;/h1&gt;
  &lt;div id=&quot;toggleButton&quot; class=&quot;toggleButton&quot;&gt;Show Content&lt;/div&gt;
&lt;/div&gt;
&lt;div id=&quot;toggledContent&quot; class=&quot;toggledContent hide&quot;&gt;This cotent area can contain anything - usually it is a menu of some sort.&lt;br&gt;&lt;br&gt;The technique used involves adding or removing a class from the node you are looking to hide or show, respectively.&lt;/div&gt;</code></pre>
</div><script async src="//codepen.io/assets/embed/ei.js"></script>

Observe the toggledContent tag includes a "hide" class.  This is necessary since we would like the default state of the div to be hidden.

## Step 2: the CSS

Next, you will need to define the classes.  Although tangential to this post, you will notice that I subscribe to the notion of never using ID's to style the code, even if there is only one ID using a single class.  You can read more about it [here](http://screwlewse.com/2010/07/dont-use-id-selectors-in-css/) and [here](http://css-tricks.com/a-line-in-the-sand/).

<div data-height="414" data-theme-id="8299" data-slug-hash="LcIKJ" data-default-tab="css" data-user="gloparco" class='codepen'><pre><code>body
	{
	background: #fff;
	font-family: OpenSans;
	}

h1
	{
	padding: 0;
	margin: 20px 0;
	font-size: 20px;
	color: #090;
	}

.mainContent
	{
	position: absolute;
	z-index: 0;
	top: 0;
	left: 0;
	width: 320px;
	height: 480px;
	background: #fff;
	text-align: center;
	}

.toggleButton
	{
	width: 140px;
	height: 60px;
	line-height: 60px;
	margin: 0 auto;
	background: #090;
	color: #fff;
	border: 3px solid rgba(255, 255, 255, 0.5);
	border-radius: 30px;
	text-align: center;
	cursor: pointer;
	user-select: none;
	-webkit-user-select: none;
	-moz-user-select: -moz-none;
	}

.toggledContent
	{
	position: absolute;
	z-index: 999;
	top: 150px;
	left: 0;
	width: 200px;
	height: 300px;
	margin-left: -3px;
	padding: 10px;
	background: #257;
	color: rgba(255, 255, 255, 0.9);
	border: 3px solid rgba(255, 255, 255, 0.5);
	border-radius: 0 20px 20px 0;
	-webkit-transform: translateX(0);
	-webkit-transition: all .3s ease;
	}

.toggledContent.hide
	{
	-webkit-transform: translateX(-100%);
	}</code></pre>
</div><script async src="//codepen.io/assets/embed/ei.js"></script>

The important bits of this code can be seen when you scroll down to the bottom.  You will see <code class="inline">.toggledContent</code>, which contains styling as well as animation properties, transform and transition.  The transform, in this case, is used to set the position of the div when it is NOT hidden (i.e., when the <code class="inline">.hide</code> class is removed from the tag - more about this, later).  The transition is used to direct the browser which transforms are to be transitioned (in this case, 'all'), how long the transition should last (in this case, '300 milliseconds'), and how to transition (in this case, 'ease' - for more elaborate values, check out the nifty online tool [Ceaser](http://matthewlein.com/ceaser/).  Likewise, the more specific <code class="inline">.toggledContent.hide</code> contains its own transform property.  Its purpose is to shift the toggledContent div along the x-axis by -100%.  Since the starting x coordinate is 0, as defined in the "left" property of the <code class="inline">.toggledContent</code> class, the transform will effectively shift the content out of the viewport.

## Step 3: the JavaScript

Tying everything together, per usual, is your JavaScript code.  The idea here is for your toggleButton div to listen for when the <code class="inline">onclick</code> event is fired, the result of which is to show or hide the toggledContent div.

<div data-height="700" data-theme-id="8299" data-slug-hash="LcIKJ" data-default-tab="js" data-user="gloparco" class='codepen'><pre><code>var contentHidden = true,
	$toggleButton = document.getElementById(&#39;toggleButton&#39;),
	$toggledContent = document.getElementById(&#39;toggledContent&#39;);
	// equivalent jQuery code:
	// $toggleButton = $(&#39;#toggleButton&#39;);
	// $toggledContent = $(&#39;#toggledContent&#39;);

// jQuery equivalent: $toggledButton.click()
$toggleButton.onclick = function()
	{
	showHideContent();
	}

function showHideContent()
	{
	if (contentHidden)
		{
		contentHidden = false;
		$toggledContent.className = &quot;toggledContent&quot;;
		// equivalent jQuery code:
		// $toggledContent.removeClass(&#39;hide&#39;);
		}
	else
		{
		contentHidden = true;
		$toggledContent.className = &quot;toggledContent hide&quot;;
		// equivalent jQuery code:
		// $toggledContent.addClass(&#39;hide&#39;)
		}
	}</code></pre>
</div><script async src="//codepen.io/assets/embed/ei.js"></script>

Here, you will notice a function called <code class="inline">showHideContent</code>.  This function simply toggles the state of the toggledContent div.  It accomplishes this by adding or removing the <code class="inline">hide</code> class from the div tag.  The effect of doing so is to trigger the transform contained in the default <code class="inline">.toggledContent</code> class or the transform contained in the <code class="inline">.toggledContent.hide</code> CSS code.

## Putting it All Together

The UI consists of a header, a single button, and an initially hidden content area.  The button, when clicked, will toggle the state of a content area.  If it's hidden, it will show it.  If it's being shown, it will hide it.  Pretty simple, eh?

<p data-height="530" data-theme-id="8299" data-slug-hash="LcIKJ" data-default-tab="result" data-user="gloparco" class='codepen'>See the Pen <a href='http://codepen.io/gloparco/pen/LcIKJ/'>Easy Show/Hide Using CSS & JS</a> by Gene Loparco (<a href='http://codepen.io/gloparco'>@gloparco</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//codepen.io/assets/embed/ei.js"></script>

Feel free to comment on this technique or to post your own techniques for accomplishing the same thing.
