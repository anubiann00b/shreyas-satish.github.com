---
layout: default
title: Introducing WorldView, an easier way to use OpenLayers.
categories: blog
---
<div class = 'page-header'>
  <h2 class = 'article-header'>
    Introducing WorldView
  </h2>
  <div class = 'details'>
    4th May, 2012
  </div>
</div>


&#x20; <a href = "https://github.com/shreyas-satish/worldview" target="_blank">WorldView</a> is a little library I've been working on to make using <a href = "http://openlayers.org" target="_blank">OpenLayers</a> **easy**. OpenLayers is of course a great mapping library, but it can be intimidating at times to perform some basic cases even. Christopher Schmidt, one of the lead developers on OpenLayers has this to say :

> The OpenLayers API is difficult to get started with for many simple problems. It can be hard to use, confusing to start, and difficult to understand for solving simple problems. 

My first map.js looked nasty. It was filled with global variables and spaghetti code picked up from a lot of OpenLayers' example pages, StackOverflow and mailing lists. This sort of annoyed me, but I really felt the pain when I needed a simple toolbar that I could use to dynamically add features such as markers, lines etc to a map. Sure, there is the <a href="http://dev.openlayers.org/releases/OpenLayers-2.11/examples/editingtoolbar.html" target="_blank">OpenLayers Editing Toolbar</a> but I didn't find it to be easily customizable. 

Christopher also adds,

> It is crucially important to supporting the future use of the project to make the easy things easy, while maintaining the ability to make the hard things possible.

WorldView steps in here by giving you a clear and easy-to-use set of APIs to solve common use cases with maps. Importantly, it wraps/returns OpenLayers objects, so that in case you'd like to do something that WorldView does not support natively, you can still do that with OpenLayers. It also gives you a simple, customizable editing toolbar.

I took an API-driven approach to writing WorldView. I wrote down the APIs I would want to use first and then coded it out so the APIs would actually work. 

I'd like to add that, WorldView is written in <a href="http://coffeescript.org" target="_blank">CoffeeScript</a>. However, you DO NOT need to use CoffeeScript to use this library, since I've included the worldview.js file. 

I chose to write WorldView in CoffeeScript, because I loved the fact that by writing in CoffeeScript, I was automatically writing <a href = "http://www.amazon.com/JavaScript-Good-Parts-Douglas-Crockford/dp/0596517742" target = "_blank">good JavaScript</a> whilst not having to worry about the usual WTFs and with a sweet syntax. Debugging wasn't a problem at all since the JavaScript generated by CoffeeScript is very read-able. When <a href = 'http://www.html5rocks.com/en/tutorials/developertools/sourcemaps/' target='_blank'>Source Maps</a> become available, debugging CoffeeScript will be even easier.

You maybe wondering why I'm not using Leaflet. There's a <a href = 'http://gis.stackexchange.com/a/8048' target = '_blank'>great answer</a> on why OpenLayers is a superior choice when it comes to writing GIS applications. Basically, its a lot more feature-rich and a much more advanced mapping library compared to Leaflet. In addition to that, we've invested quite a bit into OpenLayers at Mapunity (where I work) and we intend to continue to use OpenLayers.

Finally, I've been using WorldView with OpenLayers at work and its made my life much easier when I'm dealing with maps.







