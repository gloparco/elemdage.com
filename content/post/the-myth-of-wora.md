+++
title       = "The Myth of WORA"
description = "Write Once, Run Anywhere - myth or reality?"
date        = "2011-02-02"
+++

For years, businesses have searched for the holy grail of the development world - the notion of being able to write a program, application, app, or whatever they're now calling it, just once, while being able to deploy it on any number of systems.  Hence the term "Write Once Run Anywhere", a.k.a. WORA.

This notion really started to gain traction, or at least publicity, in the mid-90's when Java took the business world by storm.  Through the Java Virtual Machine (JVM), companies could be assured that their valuable software assets could be reused on Windows, Solaris, Unix, Linux, or Mac operating systems.  The problem was that the implementation of the JVM varied across operating systems.  In addition, the apps created with the technologies of the day, like Applets, Swing, etc. produced clunky user interfaces.

Now today, we have a whole new set of technologies with the same old set of promises.  I don't know how many times I've heard business folks say that want to learn about this HTML5 thing and how it can bring them to the promised land of WORA.  After rolling my eyes (once I've turned away from them, of course), I proceed to explain how this is something that is more promise than reality.  Besides, says I, who would want that anyway?  Let me explain.

## Be Smart

Central to the idea of WORA is the notion that you can build a user interface once and not have to worry about it again. This may have been fine in the past when all you had to concern yourself about were desktop machines, with roughly the same visual specs (although, even that is debatable – remember VGA vs XGA vs XVGA?). But now, with the proliferation of mobile and tablet devices, we have a real mess on our hands.

For example, I can go to any Web site on my iPhone 4, even something like http://www.bbc.co.uk/. But why would I want to pinch, zoom, and scroll my way around a site designed for a much larger screen? Wouldn’t it be a better user experience if the iPhone user were presented with something targeted to their particular device, or at least class of device? Of course it would. And the BBC thinks so too, since by default, it presents cell phone users with a mobile version of their site.

So the moral of this story is, just because you can do something, doesn’t always mean it’s the right thing to do. Let me repeat that, just because you can… ah, anyway, you get the point.

## Targeting Devices

Remember two paragraphs ago when I mentioned the term “class of device”? Of course you do, it was two paragraphs ago… what’s that? ok I’ll wait for you. Anyway, this is a very important term, so let me explain what I mean by it.

There are two key factors in grouping devices together into a “class”. It is not operating system (you’ll hear this a lot — target iOS devices! target Android devices!), nor is it form factor (you’re starting to hear this a lot too — target cell phones! target tablets!). What we should really be concerned about are two things: input and output.

By input, at this point to keep it simple, I mean that a mouse is a much different input device than a finger is, and you need to account for that. Now, it is possible to make visual elements that accept both forms of input, but that may end up restricting the extent to which you can target the user experience.

By output, I mean the combination of three things: screen size, screen resolution and pixel density. Screen size obviously gives you an idea of how much “stuff” you can fit on a page. But hold on, pixel density comes into play here as well. Pixel density is measured in Pixels Per Inch (PPI) that is determined by dividing the diagonal screen size by the number of pixels displayed.

So, for instance, the iPhone 4′s retina display will give you a whopping 326 PPI, whereas a super sharp 720p 42″ HDTV will give you a surprisingly paltry PPI of 35. A better comparison might be the iPhone 4 to the iPhone 3. The earlier version has the same sized screen as its successor, but its resolution, and therefore PPI, is half of what a retina display offers (163 PPI).

What this means is that for two devices with identically sized screens, the app that you create might look substantially different on both. This may show itself in a number of ways — extra whitespace, minuscule text, buttons that are hard to tap, and so on.

So what I’m saying in a nutshell is forget about this notion of writing a user interface just once and forgetting about it. Sure it will work, but you’ll have an awful lot of complaints once you release your product (or worse, no customers at all).

## What You Can Do

So now that we know what you can’t, or rather, shouldn’t do, you may be asking is there anything that can be written once? And fortunately, the answer is yes.

First off, the whole point of the previous section, was to show how classes of devices could be targeted together. So, while this doesn’t create a “write once” scenario, it does provide for a “write a few times” situation.

Secondly, what we’ve been talking about is the user interface and the overall user experience. What we haven’t mentioned is all the other “stuff” that constitutes a complete application. Things like events, functions, object models, business logic, and the like can all be reused.

This is where the promise of HTML5 (or HTML, as they now call it) comes into play. Remember, HTML is a misnomer. What we’re really talking about is a set of Web technologies; namely HTML, JavaScript, and CSS. Using these technologies, you can absolutely reuse a good portion of your code.

For example, I am currently working on a project where we’re utilizing backbone.js as the MVC framework. The MVC pattern certainly lends itself nicely to segregating what is reused and what needs to be targeted. Any backbone.js Models, Collections, Events, or Views (which are, oddly enough, really controllers in the traditional sense), can be reused across UI’s. Then, through the use of templates, CSS, or both, one can target the UI to specific classes of devices, as mentioned above.

## New Term

In the end, although WORA is pie in the sky stuff, it’s still nice to know that there are some things that can be reused. And of course, some reuse, as realized when deploying Web Apps, is preferable to no reuse, as is typically realized when deploying native apps.

How about a term to sum this all up: **WUFTEEORA** (Write the UI a Few Times and Everything Else Once, Run Anywhere). Catchy, ain’t it?
