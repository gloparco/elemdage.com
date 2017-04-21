+++
title       = "One Man's HTML5 Developer Workflow"
description = "Here's one way to develop HTML websites and apps"
date        = "2012-01-19"
+++

We are now squarely in the age of HTML5; or the age of HTML5, JavaScript, and CSS3, if you prefer. That being the case, it amazes me that for those poor souls who are new to the world of front-end development, there is little written on what their developer workflow might look like. With them in mind, I am offering up a starting point, based on my own experience and preferences.

<img title="HTML5 Workflow" src="/html5workflow.png" width="600" height="450" />

## Hardware/OS

I spent the better part of 20 years on Windows-based machines, and I don’t have one fond memory to share. If you’re into constant troubleshooting and tweaking, then by all means go Windows.

However, aside from my personal preference for Macs, there is one very good reason why you should seriously consider doing all of your development on one: iOS development. The only way you can develop for an iPad or iPhone is by using Xcode on a Mac. Since that is the case, who wants to have to develop on more than one machine? Not me, so Mac it is! (thankfully)

## Design

![Pixelmator](/pixelmator.png) For design, I use two tools extensively. For interactive mockups, I use Keynote with templates from [Keynote Kung-Fu](http://keynotekungfu.com/), although templates from [Keynotopia](http://keynotopia.com/) are equally impressive. You’d be surprised how easy it is to create a very rich, professional looking demo using Keynote.

For all of my graphics design work, I rely on the excellent [Pixelmator](http://www.pixelmator.com/). Using this tool, I can create anything I need for my Web or mobile Apps. The latest version even has support for vector graphics.

If you are into responsive design (and you should be), you should look into the usage of SVG graphics instead of raster/bitmap graphics. If you decide that’s the direction you want to go, then Pixelmator at this point can’t help you. You see, although you can create vector images within the tool, you currently cannot export such graphics to a usable format (i.e., SVG).

![Inkscape](/inkscape.png) Therefore, you’ll need to add another tool to your toolbox. I am currently looking at a free, open source tool called [Inkscape](http://inkscape.org/). It’s interface is not much to look at, but it seems to have enough features to get the job done. Alternatives include [Adobe Illustrator](http://www.adobe.com/products/illustrator.html) and [Corel Draw](http://www.corel.com/corel/category.jsp?rootCat=cat20146&cat=cat3430091). Warning: be prepared to shell out some dough for either.

## Development – Editor

![Sublime](/sublime.png) For development, I prefer a basic text editor with syntax highlighting, auto-completion, and customization options. The reason I prefer a text editor over a seemingly more rich Integrated Development Environment (IDE), such as eclipse, is that I don’t find IDE’s more feature rich at all, and IDE’s tend to be bloated and cumbersome to boot.

My editor of choice is [Sublime Text 2](http://www.sublimetext.com/2).

Sublime Text is, quite frankly, the best editor I have ever used. It not only enhances my productivity, but it looks good doing it. Aesthetics aside, there are other, more compelling reasons to seriously consider this fine piece of software. Here are just a few out of dozens one could list:

### Speed

Do you hate the Mac beach ball as much as I do (you know, that colorful spinning wheel that shows up whenever the Mac is busy)? If you do, then you owe it to yourself to download a copy of Sublime right now. It is fast – really, really fast!

There’s fast file switching, fast scrolling of large files, fast search of one or many files, fast loading of large files. Everything you do in Sublime is quick; there’s no waiting for anything. You can have 20 tabs open at a time, and guess what? It’s still just as responsive as when you have only one tab open.

### Multi-selection

I was blown away when I first saw this demonstrated in an [article](http://net.tutsplus.com/tutorials/tools-and-tips/sublime-text-2-tips-and-tricks/) by Jeffrey Way. Basically, it allows you to highlight and/or place cursors on multiple parts of the document, at which point, you can make many edits at once. A real time saver for me has been variable replacement using multi-selection. Using the search function, I can find all instances of a variable (nothing new). Using ‘find and replace’ in a traditional editor limits you to simple replacements or causes you to have to be a regex expert. Such is not the case with Sublime – perform a search, select ‘find all’, and presto! you now have each instance highlighted, with a cursor next to it, allowing you to make any changes to all instances at once, no matter how complex they may be.

### Build System

With the built-in build system, you can launch any type of app you’d like, via a menu or hot-key combination (usually F7), or even automatically after saving a file. So, for instance, I have a build system for CoronaSDK that will automatically launch the Corona simulator whenever I save changes to my lua files.

I haven’t yet set up a build system for HTML5/JavaScript/CSS. There’s so much flexibility on how to set it up, I still haven’t decided on a solution. What I’d like to do is kick off a build every time I save one of my project files. The build would then compile [.less files](http://net.tutsplus.com/tutorials/tools-and-tips/sublime-text-2-tips-and-tricks/) into .css files as needed, minify javascript files, create auto-generated docs as needed, run test scripts as needed, and then open up or refresh the browser, so I can see my changes. If there are any Sublime experts out there reading this, I’d love to know how to get this to work. I believe it can be done though.

### Plug-ins

One of the main strengths of the tried and true TextMate editor has been its plugin capabilities, and the availability of a vast array of third party plugins that have been developed over the years. Sublime is fully compatible with nearly all of TextMate’s plug ins. In fact, I should rephrase by saying, I haven’t found one TextMate plugin that isn’t compatible, although I do have one that gives me a warning each time I launch Sublime (the CoronaSDK plugin for some reason).

In addition, Will Bond has created the excellent ‘Package Control’ plugin, which allows you to easily discover and install other plugins. This is the first plugin that everybody should install.

From there, you can install any of a myriad of available plugins. If you can dream it up, chances are there is a plugin for it already. And if by some off chance there is not, then Sublime makes it easy enough to create your own.

Here are the plugins that I use regularly:

[Sublime SFTP](http://wbond.net/sublime_packages/sftp): another excellent plugin by Will, this allows me to save my files and projects to my remote server without having to fire up Filezilla or the Terminal. One cool feature is the auto-save option. I have it set up so that when I save any of my files locally, they are automatically pushed to my server as well. This comes in handy when I want to test some of my code on an iPad for instance.

I need to give Will some props here. The guy is a very responsive, available developer – case in point: before I gladly paid the $16 license fee for this plugin, I emailed Will asking if he could add support for the case where an external tool or build process auto generates a file, such as in my case where a LESS compiler auto-generates a CSS file. While Will was somewhat handcuffed in what he could do, nonetheless, he came up with a solution in his very next build and now this plugin’s file monitoring feature is something I use regularly.

[SublimeLinter](https://github.com/Kronuz/SublimeLinter): a [JSHint](http://www.jshint.com/) plugin that is invaluable in helping me detect JavaScript errors.

[SideBarGit](https://github.com/SublimeText/SideBarGit): this adds basic and some advanced git functionality to the sidebar, allowing you to perform commits and other git commands without leaving the editor.

[My own theme](http://blog.elemdage.com/wp-content/uploads/2012/01/Theme-Gene.zip): although I like a lot of the visual themes that are out there already, most of them tend to be light text on a dark background. If I’m coding for quite a while, I tend to prefer dark text on a light background. None of the themes really struck my fancy, so I went ahead and created my own. Here is a screenshot of an HTML5 page:

<img title="Sublime ScreenShot" src="/SublimeScreenShot.png" width="640" height="394"/>

If anyone is interested in my theme, feel free to download it, here: [Theme – Gene](http://blog.elemdage.com/wp-content/uploads/2012/01/Theme-Gene.zip)

### Notable Editor Alternatives

[TextMate](http://macromates.com/): decent, but outdated de-facto standard for many developers; the new [2.0 alpha](http://blog.macromates.com/2011/textmate-2-0-alpha/) version is finally out after years in the making, but compared to Sublime, it looks like ‘too little, too late’

[MacVim](http://code.google.com/p/macvim/): it’s Vim, need I say more? ;-) Actually, I do need to say more: I hate, hate, hate, hate, hate Vim – did I mention that I hate it? I just don’t get how anyone could like the antiquated Unix-originating Vim with it’s stupid modes, over any of the other options that are out there. Emacs was waaay better than Vim back in the day; nano is better than Vim now; and they both pale in comparison to Sublime, and the other feature rich editors listed here; and yet, excellent coders, such as Thomas Fuchs use this editor — like I said, I don’t get it

[BBEdit](http://www.barebones.com/products/bbedit/index.html?utm_source=thedeck&utm_medium=banner&utm_campaign=bbedit): It’s nice, but it just isn’t as snappy, full featured, or nice to look at as Sublime.

[TextWrangler](http://www.barebones.com/products/textwrangler/): BBEdit’s little brother. It might be the best free editor out there, but lacks many of the features the others have.

### Notable IDE Alternatives

[Dreamweaver](http://www.adobe.com/products/dreamweaver.html): I nearly hate Dreamweaver as much as Vim. Actually, I might even hate it more. I have never seen a more bloated, slow, jumbled mess of an application in my life. It’s a memory hog, as are most Adobe products, but unlike FlashBuilder, it’s interface and functionality does not even come close to making up for it. And get this – they’re charging $400 for this piece of garbage! Stay away; stay far, far away.

[Aptana Studio](http://aptana.com/): if you like Eclipse, you might like Aptana. I don’t like Eclipse – ’nuff said.

[Coda](http://panic.com/coda/): has issues with large files; generally slow and bloated, albeit not as much as Dreamweaver or Aptana.

[Espresso](http://macrabbit.com/espresso/): used the trial version and was underwhelmed.

[NetBeans](http://netbeans.org/): a free, open source IDE that people I know use. Not for me, though.

[WebStorm](http://www.jetbrains.com/webstorm/): cheezy name, no doubt, but a lot of commenters, below, seem to like it.

## Development – Supporting Tools

![CodeKit](/codekit.png) In lieu of using Sublime’s built in build system to compile my .less files and refresh my browser, I am currently using [CodeKit](http://incident57.com/codekit/) to do the same. CodeKit does some other things like running JavaScript through jshint, but since I’m already doing that in Sublime, I don’t really need that feature. The only complaint I have for CodeKit is that, while it will auto reload the browser whenever you change your .less or .html files, the tool does not auto update whenever I make changes to my JavaScript files. I’m not sure if this is a case of user error, or if it’s a limitation of the tool, but most of my code changes are done in JavaScript, so that would be a nice feature to add. EDIT: Per the author’s comment, below, this issue has been fixed.

There are alternatives to CodeKit that do much the same thing and are worth checking out. One such alternative is [SimpLESS](http://wearekiss.com/simpless), but there are others as well.

## Debugging

I use Safari as my test browser, making use of their excellent developer tools. For those who don’t know, these built-in tools allow you to inspect your scripts, set code break-points and watch expressions, view the debug console, and more. It’s really an invaluable tool.

To debug mobile apps, there is nothing like Safari’s tools available. One interesting solution has piqued my interest though. It’s called [weinre](http://phonegap.github.com/weinre/), which is not a hot dog substitute, but rather a "we"b "in"spector "re"mote, hence the name.

![Resize Plugin](/resize.png) In addition, I use but one Safari plugin – [Resize](http://resizesafari.com/) by Chen Luo. It allows you to quickly resize your browser to pre-set exact dimensions. Chen has built in nearly every dimension you’d be interested in: the iPhone’s 320×480, the iPhone retina’s 640×960, the iPad’s 1024×768, and a ton of others. For those not willing or able to shell out the $9 for this excellent plugin, Chen also provides a free website that works similarly, albeit by opening a new browser window instead of resizing the current window. It’s called [resizeMyBrowser](http://resizemybrowser.com/).

## Testing

For JavaScript development, unit testing is desirable. I have to admit, however, that I haven’t really standardized on one tool as of now. I am currently looking at several helpful libraries and tools, including [testling](http://www.testling.com/) and the straightforward [Unit Test](https://gist.github.com/976405) library.

For mobile development, you’ll need to use emulators. For iOS, there are the emulators that come with Xcode. For Android, Google provides an [emulator](http://developer.android.com/guide/developing/tools/emulator.html). If you want to go further than that and test on specific device emulators, there’s Adobe’s [Device Central](http://www.adobe.com/products/devicecentral.html).

## Doc Generators

I’m not sure if most people really need doc generators (myself included). Proper coding techniques and naming conventions should provide for self-evident logic enlightenment.

That being said, when working on a large team, or when creating re-usable libraries or API’s, documentation is a must. There currently seems to be no de-facto standard for JavaScript doc generation, as is the case in, say Java (with the venerable JavaDoc). So, here is my pick of the litter for those interested:

[JSDoc2](http://code.google.com/p/jsdoc-toolkit/): the original JSDoc has been deprecated, so you may choose from this version, or [JSDoc3](https://github.com/micmath/jsdoc), currently in beta.

[YUIDoc](http://developer.yahoo.com/yui/yuidoc/): I like the default output of this tool better than JSDoc, but it’s still not perfect.

[PDoc](http://pdoc.org/): the output that it generates is the best of the three listed here, but I’m not sure how it will do with non-Prototype code (I think it should work, but I’m not positive).

[docco](http://jashkenas.github.com/docco/): if you’re looking for something a little different, you may want to consider docco. Its output consists of two panes – one with the code, and the other with comments mapped to the code. I haven’t seen it used anywhere, except in the documentation of the excellent JS MVC library [backbone.js](http://backbonejs.org/).

## Version Control

You should get used to using version control, even if you’re a solo developer. It’s a good habit, and chances are, sooner or later, you’ll want to share your code or collaborate with others. Any version control product will do, but the two you should be most educated on at this point are git and svn.

## Mobile Deployment

![PhoneGap](/phonegap.jpg) There will no doubt be many cases when you’ll want to deploy your HTML5 app to devices other than the browser. In such cases, you could let mobile users access your site via their web browser. Or, you could package up your code into a native shell, thereby creating what is known as a “hybrid app” (although this term can mean any number of things, depending on whom you ask).

To create such hybrid apps, you basically have two choices: [PhoneGap](http://phonegap.com/), or [Titanium](http://www.appcelerator.com/products/titanium-cross-platform-application-development/). I prefer the simplicity and larger developer community of PhoneGap (a.k.a., Apache Cordova – yeah, good luck with that name change!). But both have their place and their supporters.

![TestFlight](/testflight.jpg) Once you have built your hybrid app, it’s deployed to your app store of choice by whatever means you would normally submit a native app. If you first want to beta-test your hybrid app, then I recommend the über-cool [TestFlight](https://testflightapp.com/), which makes the otherwise painful process of distributing your app to beta-testers a breeze.

I should also mention [AppMobi](http://www.appmobi.com/) here for completeness, but as I state in the comments, below, I was put off by their message board postings on their site.

## Summary

I’ve covered a lot of ground here, going for breadth rather than depth. That being said, I hope that this was a useful resource for those looking to piece together the often confusing world of HTML5 development.

I would love to hear what your favorite tools are and what your development workflow is. I am always open to learning about new tools or techniques and will gladly update this posting as I refine my own workflow even further.
