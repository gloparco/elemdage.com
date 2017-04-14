+++
title       = "HTML5: Is it Ready for Prime Time?"
description = "HTML5 is here to stay - is it ready for production use?"
date        = "2010-05-25"
+++

The recent announcement by Apple that it has sold over <a href="http://www.apple.com/pr/library/2010/05/03ipad.html">one million iPads in just 28 days</a> has developers chomping at the bit to create apps for the iPhone OS.  However, for many of these App Store success story hopefuls, there are at least two problems that they face before writing even a single line of code.

If one would like to develop a native app for the iPhone OS, they must either take a time machine back to 1988 and learn the nasty, archaic language known as Objective-C, or they must take a leap of faith and hope that Apple’s recent <a href="http://blogs.zdnet.com/Burnette/?p=1904">Developer Agreement changes</a> don’t apply to Adobe and other vendors offering tools that translate various languages into native iPhone code.

If instead, one would like to develop a more portable app, designed to run on most any device, there is one technology that has produced more buzz than a hummingbird on steroids.

Enter HTML5, the apparent panacea of the software industry.  Is it supported by iPhones and iPads?  Check!  What about Android?  Yup!  And those old clunky things we still use at our desks and lug around in our travel bags, what are they called again?  Oh yeah, computers – do they support HTML5 apps?  They sure do!

So, then problem solved, right?

Well, not so fast.  As nice as it would be to code an app that can be run on any platform, there are some things to consider before drinking the HTML5 Kool-Aid.

## Are we done yet?

The <a href="http://dev.w3.org/html5/spec/Overview.html">HTML5 specification</a> is, hmm how shall I put this… still in its suggestion phase, otherwise known as a “working draft” by the W3C, the braintrust behind the spec.  The authors, in the third paragraph of the most recent draft, even go so far as to state “Implementors should be aware that this specification is not stable.”  Really?  And developers are still expected to get excited about using HTML5 in professional, production-ready apps?

## Get me out of this thing!

HTML5 is still bound to the browser, and as such is somewhat restricted in what it can do.  In addition, developers are at the mercy of the browser vendors, who get to decide which aspects of the HTML specification will be supported and which will be left out.  Most good browser vendors are ahead of the curve, supporting much of the spec already, and planning to support many more features in time.  Others seem to be more reluctant and slow moving with their adoption (yes, I’m talking about you, Microsoft).

So as a result, HTML5 developers are forced to either scale back their usage of certain features, taking a “least common denominator” approach, or throw caution to the wind and just hope that browser vendors will start adopting new features more rapidly (don’t hold your breath).

## It’s Déjà vu all over again

Being tied to the browser also causes another headache for developers (a headache that javascript/css developers should be intimately familiar with) – inconsistent rendering.  You can be guaranteed that the app you’ve meticulously developed for the iPad will look great when rendered by its WebKit engine on its 1024x768 screen.  You can also be guaranteed that the same app will look atrocious when rendered in IE 9 on a 1024x768 monitor, or when rendered on a Linux/Firefox laptop with a 1024x768 screen.

So then a developer must inject logic into their code that detects the OS/browser/version combination, along with code specific to each combination, to ensure that the app looks the same no matter where it is run.  And this is the future?

Why can’t there be an open source plugin, similar to Flash or Silverlight, that browser vendors must support in order to be HTML5 compliant?  That would solve all our problems!  You would get pixel perfect rendering!  Your app would be lean and mean and free of any case statements!  It would be awesome!

Why can’t we band together and demand such a solution?  Think about it, it could work!  I’ll start a petition… wait… what?  Oh yeah, I almost forgot, we’ve done that before.  It’s called Java.

Oh well, I got excited there for a moment.

## I can only do so much

What if you want your HTML5 app to be able to use the nifty features of the iPhone or iPad?  Well, aside from basic functionality, you’re out of luck, at least for now.  Device specific features such as the accelerometer, camera, compass, and multi-touch display are currently off limits to non-native apps.

## You’re so negative, I’m positive!

Although the tone of this article might lead you to believe that I am railing against HTML5, the truth is that I am very much rooting for it to succeed (and I think it will).  What I am trying to point out is that there are things to consider before jumping into the technology.

In the long run, I’d be surprised if HTML5 weren’t a huge hit and the technology of choice for app developers.  In particular the combination of the iPad and HTML5 has the potential to be a real game changer, both in the consumer realm as well as the business world.

Even in its current state, there are still some categories of apps that could benefit from using HTML5.  One such category is Enterprise RIA’s.  Such apps are typically deployed to internal users, in a controlled environment.  Having such an audience would afford developers the luxury of targeting specific OS/browser/version combinations.

If you are considering using HTML5 in your next project, take the time to weigh out the pros and cons.  And if you decide not to use it now, make sure to keep tabs on the specification’s progress, because when you have Google and Apple behind something, it’s very likely that it’s here to stay!

What do you think of the viability of HTML5?
