+++
title       = "Top 20 JavaScript Technologies: March 2017"
description = "Relative Strength Index for JS Tech (RSIJT)"
date        = "2017-03-02"
+++

![JS Logo](/js.jpg) As a follow-up to my previous post, [Top 10 Programming Languages](/top-10-programming-languages-march-2017), I thought it would be interesting to look at specific technologies in the JavaScript world.

## What's in a Name?

The title of this post is a bit misleading, as this analysis includes CSS libraries, such as bootstrap, LESS, and SASS. I was going to call it “Top 20 Full Stack Technologies” but full stack generally includes technologies such as PHP and .Net. This list only includes HTML/JS/CSS, but it includes those technologies on both the client and server side. To that end, the rating system is called Relative Strength Index of JavaScript Technologies (RSIJT).

## RSIJT Methodology

To form a list of technologies to look at, I searched GitHub for those libraries with the highest number of stars. I added any libraries that I am aware of that were not included, that might nonetheless be compelling in one way or another. “Technologies” include frameworks, libraries, languages (like ES6 and TypeScript), task runners, testing libs, UI libs, and anything else in our JS world.

The RSIJT formula factors in discussions on Stack Overflow, and job postings on Dice. It weighs two types of job postings – those which contain the technology in its title are given more weight, and those which contain the technology in its description are given a lesser weight.

To make the list relevant, the ratings are computed based on the last month’s worth of data.

The technologies included in this analysis include:

    AMD, angular2, angularJS, babel, backbone, bootstrap, bower, chart.js, coffeescript, common.js, d3, ember.js, es6, express.js, flux, foundation, grunt, gulp, handlebars, impress.js, jasmine, jquery, karma, leaflet, less, lodash, meteor, mocha, modernizr, moment.js, mustache, node, polymer, react-native, React.js, redux, require.js, reveal.js, sails, sass, semanticUI, socket.io, three.js, typescript, underscore, vue.js, web components

## 10 Most Popular JavaScript Technologies

Following are the top 10 JS technologies in March 2017, using the RSIJT formula:

<center class="moreSpace">
    <table style="width: 50%">
        <tr><td>1.</td><td>AngularJS</td><td style="text-align:right">79.3</td></tr>
        <tr><td>2.</td><td>jQuery</td><td style="text-align:right">61.2</td></tr>
        <tr><td>3.</td><td>Node.js</td><td style="text-align:right">55.1</td></tr>
        <tr><td>4.</td><td>React</td><td style="text-align:right">38.9</td></tr>
        <tr><td>5.</td><td>AngularJS 2</td><td style="text-align:right">23.4</td></tr>
        <tr><td>6.</td><td>Bootstrap</td><td style="text-align:right">13.6</td></tr>
        <tr><td>7.</td><td>TypeScript</td><td style="text-align:right">8.1</td></tr>
        <tr><td>8.</td><td>React Native</td><td style="text-align:right">5.7</td></tr>
        <tr><td>9.</td><td>Backbone.js</td><td style="text-align:right">5.5</td></tr>
        <tr><td>10.</td><td>Express</td><td style="text-align:right">4.6</td></tr>
    </table>
</center>

No surprises here. Angular and React are by far and away the most popular front end frameworks. Ember just missed the cut and I expect vue.js to climb the list over the coming months.

Also mixed in are what I consider legacy JS tech (in the JS world, legacy means it’s old tech after just 5 years!). Libraries like jQuery, Bootstrap, and Backbone are on this list, not because they are the latest and greatest, but because they are used in so many existing apps.

Node.js and Express continue to be very popular technologies on the server side.

## Next 10 Most Popular JavaScript Technologies

As a bonus, I have decided to include the next 10 technologies with their RSIJT score.

<center class="moreSpace">
    <table style="width: 50%">
    <tr><td>1.</td><td>Ember.js</td><td style="text-align:right">4.6</td></tr>
    <tr><td>2.</td><td>D3.js</td><td style="text-align:right">4.0</td></tr>
    <tr><td>3.</td><td>Sass</td><td style="text-align:right">3.9</td></tr>
    <tr><td>4.</td><td>Redux</td><td style="text-align:right">3.7</td></tr>
    <tr><td>5.</td><td>ES6</td><td style="text-align:right">3.4</td></tr>
    <tr><td>6.</td><td>Vue.js</td><td style="text-align:right">2.8</td></tr>
    <tr><td>7.</td><td>gulp.js</td><td style="text-align:right">2.5</td></tr>
    <tr><td>8.</td><td>Less.js</td><td style="text-align:right">2.4</td></tr>
    <tr><td>9.</td><td>Jasmine</td><td style="text-align:right">2.1</td></tr>
    <tr><td>10.</td><td>Grunt</td><td style="text-align:right">2.0</td></tr>
    </table>
</center>

Over time I will be revising the list and formula. If you have any suggestions on how to make this more accurate or useful, or if you know of other JS tech that should be included in the analysis, please drop me a line!
