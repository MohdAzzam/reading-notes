# Images 

`<img src=""/>`
------------------------------------------------------ 
Controlling sizes of images in CSS using `width and hight` properties . 
Image is inline element we can change his properties using `display:block` we can also float image using `float` properties 

-------------------------------------------------------
Background images can appear just once or be repeated across the background of the box.
    specify the dimensions of images using CSS.
    we can add `background-image` to our background web page .
    we can repeating background image using `background-repet`
    we can play arround postion of background-postion using `background-postion`
    we can use the shorthand `background`  to specify the all element we descius it .


This is very helpful when you use the same sized
images on several pages of your site.

Images can be aligned both horizontally and vertically
using CSS.

We can use a background image behind the box
created by any element on a page.


We can create image rollover effects by moving the
background position of an image.

To reduce the number of images your browser has to
load, you can create image sprites.


# Practical Information
Search Engine Optimization (SEO)
Search engine optimization (or SEO) is the practice of trying to help your site appear nearer the top of search engine results when people look for the topics that your website covers. 
-----------------------------------------------
* On-Page SEO
  1. page title
  2. url web-address
  3. heading 
  4. Text
  5. Link Text
  6. Img alter text
  7. page description 

How to Identify Keywords and Phrases
1. Brainstorm
2. Organize
3. Research
4. Compare
5. Refine
6. Map

Analytics: Learning about your Visitors

How Many People Are Coming to Your Site?

What Are Your Visitors Looking At?

Where Are Your Visitors Coming From?

Domain Names & Hosting

FTP & Third Party Tools 

### Summary 

* Search engine optimization helps visitors find your sites when using search engines.
 
* Analytics tools such as Google Analytics allow you to see how many people visit your site, how they find it, and what they do when they get there.
 
* To put your site on the web, you will need to obtain a domain name and web hosting.
 
* FTP programs allow you to transfer files from your local computer to your web server.
 
* Many companies provide platforms for blogging, email newsletters, e-commerce and other popular website tools (to save you writing them from scratch).

----------------------------------------------------------------------------

# Video and Audio APIs

HTML5 comes with elements for embedding rich media in documents — `<video>` and `<audio>` — which in turn come with their own APIs for controlling playback, seeking, etc. This article shows you how to do common tasks such as creating custom playback controls.

------------------------------------------------------------------------------

The `<video>` and `<audio>` elements allow us to embed video and audio into web pages. 

`<video controls>`
  `<source src="rabbit320.mp4" type="video/mp4">`
  `<source src="rabbit320.webm" type="video/webm">`
  `<p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>`
`</video>`


#### The HTMLMediaElement API

Part of the HTML5 spec, the HTMLMediaElement API provides features to allow you to control video and audio players programmatically — for example `HTMLMediaElement.play()`, `HTMLMediaElement.pause()`, etc. This interface is available to both `<audio>` and` <video> `elements, as the features you'll want to implement are nearly identical.



