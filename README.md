#<a id="docs" href="#docs">ASFramework - HTML</a>

###Version 0.0.1 In Development


NOTE: this is IN DEVELOPMENT AND SUBJECT TO FREQUENT CHANGE

Playing around with SCSS trying to create a responsive framework using media queries and a fluid layout.

Lightweight Package size
Real weight of linked files - 4MB
full download - 11MB
Google pagespeed score 98 out of 100

full download is 11MB however the weight of the files actuallly linked and used is 5MB. This is because i've included fallbacks for jquery and jquery-ui in case Googles cdn goes down. And also because for each plugin i have included the full install including demo pages, manuals and demo images. These wont ever actually run on your site, they're just for your reference.


Features

Adaptive design using a fluid 100% width and media queries at 1000px and above, 768px to 999px, 480px to 767px and 479px and below.

Images are responsive and take up the amount of space given to them by default, use your own css selectors to define 

plugin - jQuery.retina.js if the browsers devicepixelratio is 2 or more (retina or hi res) automatically swaps out images for their retina versions as defined by the @2x convention. if non retina doesnt load both images, if retina it does but the user will only see the retina version. This means it has minimal impact on the majority who don't have retina screens. by @mcilvena http://mcilvena.com/articles/jquery-retina/

Plugin - jquery + jquery-ui provided from Googles CDN, with local fallbacks.

Plugin - Modernizr feature detection, recommended tests given by the webshims installation guide.

Plugin - Webshims Lib polyfills features in older browsers. Can be set to polyfill all features it can or specific features only. default is all, this results in a small impact on page load.

plugin - ResponsiveSlides.js v1.54 lightweight image slider. slider will by default take up the full 100 width, use slider-sizing divs to set the size/margins/borders

plugin - FitVid.js uses jquery to resize youtube,vimeo,blip.tv, viddler & kickstarter videos. wrap a videos iframe  or embed in the video sizing & video-container divs. use the video-sizing divs to set the size/margins/borders. the video-container will be 100% width of the video-sizing

plugin -jPanelMenu.js enables a mobile off canvas menu when a trigger is clicked. simple operation that doesnt require you to change up your html, with plenty of options http://jpanelmenu.com

script - smooth scrolling from http://www.paulund.co.uk/smooth-scroll-to-internal-links-with-jquery

Server - gzip enabled in .htaccess if your server supports it.

Server - Apache2 mod_expires & mod_headers browser caching enabled in .htaccess if your server supports it. Using Etags however they can be disabled.

stylesheet - custom animate.css transitions and effects, not linked by default but included.

Dreaded IE8 support - added a conditional ie* stylesheet, ie8 doesnt support media queries so ill use this to set a fixed width of 1000px

Notes

-removed the skipser youtube embed script as it breaks with responsive videos. need another lazy loading solution.

#<a href="#license" id="#license">License</a>
This is released under GPL and/or MIT licenses (i know zero about licenses)for what its worth feel free to use, abuse, deconstruct, fork, or distribute my work both for private or commercial use. Send me a tweet if you do, that'd make me a happy lad. Of course each of the plugins or third party code used will of course have their own licenses you may want to check.