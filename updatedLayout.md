# Layout

#### Building Blocks
Css treat each HTML elements as a box 
-------------------------------
There are two key concepts in postioning elements 

1. Block : `<h1> <p> <ul> <li> ` 
2. Inline  `<img> <b> <i>` 
   
--------------------------------

Containing element : if block sit on another block elements then the outer box that called `containing` or `parent` elements 

#### Postion Schemas 

1. Normal Flow :block elements apper on new line  
2. Relative Postion: moves element from the normal position it shift to the `top right bottom left`
3. Absolute Postion : not follow any postion 
4. Fixed Postion : it fixed the element postion and dont affect another element postion 
5. Floating element : allow us to take element out of his flow 
    - after float the element and finished with float properties we should use this properties to removeing the float `clear : both` 

When we move any element from normal flow we can overlap The `Z-index` property 
which box appers on top 


#### Screen Sizing 
----------------------
Different visitors to your site will have different sized screens that show
different amounts of information, so your design needs to be able to
work on a range of different sized screens.


#### Page Sizing
Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide
(since most users will be able to see designs this wide on their screens).

Fixed Width Layouts : the page will show with the same size on any screen 
Liquid Layouts : the page will fit the all  screen 


### Layout Grids
Grids divide the page into more than one part `960 Pixel wide 12 Column Grid`

----------------------


##### Multiple Style Sheets 
1. using `@import url('css/somestyle.css')`
2. using `<link rel="stylesheet" type="text/css" href="css/somestyle.css" `
   

--------------------------------------------

# Summary 
* `<div>` elements are often used as containing elements to group together sections of a page.
* Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.
* The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)
* Pages can be fixed width or liquid (stretchy) layouts.

* Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).
* Grids help create professional and flexible designs.
* CSS Frameworks provide rules for common tasks.
* You can include multiple CSS files in one page.