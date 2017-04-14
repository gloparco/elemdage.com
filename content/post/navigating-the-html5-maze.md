+++
title       = "Navigating the HTML5 Maze"
description = "HTML5, JavaScript, and CSS have so many libraries, it will make your head spin.  This blog post tries to make sense of it all."
date        = "2012-05-29"
+++

<p style="text-align: left;">Ember! Batman! Spine! Knockout! Bootstrap! Boilerplate!  No, this is not the opening sequence to a bad B-list movie from the 1960's.  It is but a very small sampling of the overwhelming number of HTML5 libraries/frameworks/(insert your own catagorization here) available for use by unsuspecting, bright-eyed developers.  [Note: remember, when I use the term HTML5, it is based on what seems to be the industry accepted use of the term which encompasses HTML5, JavaScript, and CSS3]

Selecting one or more open source projects to make your development life easier usually ends up being a project in and of itself.  Witness this conversation that may seem all to real to a number of you reading this:</p>
<p style="text-align: left;"><strong>Developer A:</strong> "I think we should use jQuery for our next project."</p>
<p style="text-align: left;"><strong>Developer B:</strong> "But it's a mobile project using HTML5.  Wasn't jQuery built before HTML5 and mobile?"</p>
<p style="text-align: left;"><strong>Developer A:</strong> "So what about jQuery Mobile?  That came later, right?"</p>
<p style="text-align: left;"><strong>Developer B:</strong> "Yes, I think so... but that's only part of the puzzle - I've heard good things about HTML5 Boilerplate."</p>
<p style="text-align: left;"><strong>Developer A:</strong> "Oh yeah, me too!  I saw that Irish guy post something on Twitter about that.  Now that should solve our problems!"</p>
<p style="text-align: left;"><strong>Developer B:</strong> "Speaking of Twitter, I've also heard good things about Twitter's Bootstrap library - if it's good enough for Twitter, it should be good enough for us, don't you think?"</p>
<p style="text-align: left;"><strong>Developer A:</strong> "Yeah, good point.  Speaking of being good enough for established companies, I heard Apple uses Sproutcore, and that there are a ton of companies using something called Backbone"</p>
<p style="text-align: left;"><strong>Developer B:</strong> "I'm pretty sure Sproutcore has been replaced by Amber or Ember or something, but I can't remember.  Backbone seems to have a large following, you're right.  What about templates?  We need templates, don't we?"</p>
<p style="text-align: left;"><strong> Developer A:</strong> "I'm sure we will, so how about Mustache or Handlebars?  Will they play nicely with anything we've mentioned so far?"</p>
<p style="text-align: left;"><strong> Developer B:</strong> "I have no idea.  Maybe we should just write everything from scratch.  That will be a lot simpler and cleaner anyway."</p>
<p style="text-align: left;"><strong>Developer A:</strong> "Sounds good to me.  Who knows how long these libraries will be around anyway."</p>
<p style="text-align: left;">I think you get the idea by now.  For many of us, Developer A and Developer B are the same person, and this whole conversation takes place within the confines of one's head (come on - I can't be alone here, can I!?).  Unfortunately, there are no simple roadmaps for confused people like me, who might have a pretty good idea of where they want to go, but no clue on how to get there.  What ends up happening then, for many anlytical sorts, is the dreaded paralysis by analysis, where nothing gets done for weeks or possibly longer.</p>
<p style="text-align: left;">I'd like to try to help my fellow developers by putting a stake in the ground and declaring 'THE best' solution, given a specified use case.  Of course the answer I give will have many more people who deem it wrong than right, but that's a risk I'm willing (silly enough?) to make.  After all, these frameworks are all top-notch in my book, so you really can't go wrong with any selections in most cases.  The intended value of my reommendations lies in not having spend countless hours in research.</p>
<p style="text-align: left;">Once the flames from the comments have died down (Ember, anyone? --sorry, couldn't resist), I might even try to expand on this with more use cases and/or more selection criteria.  We'll see how that goes.  Ok, flame suit on:</p>

<hr style="text-align: left;" />
<p style="text-align: left;"><strong><em>You want:</em></strong> nothing more than a simple tempting system</p>
<p style="text-align: left;"></p>
<p style="text-align: left;"><strong><em>Go get:</em></strong> <a href="http://handlebarsjs.com/">Handlebars.js</a></p>

<hr style="text-align: left;" />
<p style="text-align: left;"><strong><em>You want:</em></strong> nothing more than a simple MVC framework</p>
<p style="text-align: left;"></p>
<p style="text-align: left;"><strong><em>Go get:</em></strong> <a href="http://knockoutjs.com/">Knockout.js</a></p>

<hr style="text-align: left;" />
<p style="text-align: left;"><strong><em>You want:</em></strong> nothing more than a grid/layout/widget library</p>
<p style="text-align: left;"></p>
<p style="text-align: left;"><strong><em>Go get:</em></strong> <a href="http://twitter.github.com/bootstrap/">Bootstrap</a></p>

<hr style="text-align: left;" />
<p style="text-align: left;"><strong><em>You want:</em></strong> an all-in-one jQuery-centric mobile framework</p>
<p style="text-align: left;"></p>
<p style="text-align: left;"><strong><em>Go get:</em></strong> <a href="http://jquerymobile.com/">jQuery Mobile</a></p>

<hr style="text-align: left;" />
<p style="text-align: left;"><strong><em>You want:</em></strong> a starting-point collection of best practices, templates, libraries, and structure for a Web Site</p>
<p style="text-align: left;"></p>
<p style="text-align: left;"><strong><em>Go get:</em></strong> <a href="http://html5boilerplate.com/">HTML5 Boilerplate</a></p>

<hr style="text-align: left;" />
<p style="text-align: left;"><strong><em>You want:</em></strong> an Enterprise scale, highly structured, single-page, MVC-based, mobile app wrapped in a native shell</p>
<p style="text-align: left;"></p>
<p style="text-align: left;"><strong><em>Go get:</em></strong> <a href="http://phonegap.com/">PhoneGap</a>, <a href="http://emberjs.com/">Ember.js</a></p>

<hr style="text-align: left;" />
<p style="text-align: left;"><strong><em>You want:</em></strong> an Enterprise scale, flexibly structured, single-page, MVC-based mobile app, wrapped in a native shell</p>
<p style="text-align: left;"></p>
<p style="text-align: left;"><strong><em>Go get:</em></strong> <a href="http://phonegap.com/">PhoneGap</a>, <a href="http://documentcloud.github.com/backbone/">Backbone.js</a> (uses <a href="http://documentcloud.github.com/underscore/">Underscore.js</a>), <a href="http://html5boilerplate.com/mobile">Mobile H5BP</a> (comes w/<a href="http://jquery.com/">jQuery</a>)</p>

<hr style="text-align: left;" />
<p style="text-align: left;"><strong><em>You want:</em></strong> a small to medium scale, MVC-based mobile app, wrapped in a native shell</p>
<p style="text-align: left;"></p>
<p style="text-align: left;"><strong><em>Go get:</em></strong> <a href="http://phonegap.com/">PhoneGap</a>, <a href="http://knockoutjs.com/">Knockout.js</a></p>

<hr style="text-align: left;" />
<p style="text-align: left;"><strong><em>You want:</em></strong> a large-scale Web Site that works on 90% of desktops, tablets, and laptops - even IE6</p>
<p style="text-align: left;"></p>
<p style="text-align: left;"><strong><em>Go get:</em></strong> <a href="http://html5boilerplate.com/">HTML5 Boilerplate</a>, which comes with the excellent <a href="http://www.modernizr.com/">Modernizr</a>, and <a href="http://jquery.com/">jQuery</a></p>

<h2 style="text-align: left;">Find what you're looking for?</h2>
<p style="text-align: left;">Please feel free to leave your comments on this very subjective list, and be sure to add your own recommendations, or requests for a recommendation.  For any such requests, I'll be happy to update this post with my suggestions.</p>
