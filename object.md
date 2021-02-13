# Object 

What is an Object ?

Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object,
variables and functions take on new names.

- IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES
- IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS

`    let hotel = {`
       ` 'name': 'Azzam',`
       ` 'rooms': 40,`
       ` 'booked' : 30 ,`
       ` 'gym':true,`
       ` 'roomTypes':['wwin','double','suite'],`
     `   checkAvailability : function (){`
       `     return this.rooms->this.booked;`
   `     }`
 `   } `

* Programmers use a lot of name/value pairs:
  1. HTML uses attribute names and values.
  2. CSS uses property names and values.
  
* In JavaScript :
  1. Variables have a name and you can assign them a value of a string, number, or Boolean.
  2. Arrays have a name and a group of values. (Each item in an array is a name/value pair because it has an index number and a value.)
  3. Named functions have a name and value that is a set of statements to run if the function is called.
  4. Objects consist of a set of name/value pairs(but the names are referred to as keys).


Creating AN OBJECT :
    1. Literal notatiion : literal notation is the easiest and most popular way to create object.

Accessing An Object and dot notation 
    * you can access the properties using dot notation 
    * You can also access just the  properties using sequare brackets not a method 
    ` let hotelName = hotel.name;`
    `let roomsFree = hotel.checkAvailability();`
    `let hotelName=hotel['name'];`










# Document OBJECT MODEL 
> The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.


THE DOM TREE IS A MODEL OF A WEB PAGE
> As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes.


`<html>`
`<body>`
`<div id="page">`
`<hl id="header">List</hl>`
`<h2>Buy groceries</h2>`
`<ul>`
`<li id="one" class="hot"><em>fresh</em> figs</li>`
`<li id="two" class="hot">pine nuts</l i>`
`<li id="three" class="hot">honey</l i>`
`<l i id="four">balsamic vinegar</l i>`
`</ ul>`
`<script src="js/l i st. js "></scri pt>`
`</ div>`
`</ body>`
`</ html>`


WORKING WITH THE DOM TREE 

STEP 1: ACCESS THE ELEMENTS 
    1. SELECT AN INDIVIDUAL ELEMENT NODE
        * `get Element Byld ()`
        * `querySelector ()`
    2. SELECT MULTIPLE ELEMENTS (NODELISTS)
        * `getElementsByClassName()`
        * `getElementsByTagName()`
        * `querySelectorAll()`
    3. TRAVERSING BETWEEN ELEMENT NODES
        * `parentNode`
        * `previousSibling / nextSibling`
        * `firstChild / lastChild`

STEP 2: WORK WITH THOSE ELEMENTS
    1. ACCESS/ UPDATE TEXT NODES
    2. WORK WITH HTML CONTENT
    3. ACCESS OR UPDATE ATTRIBUTE VALUES




### Summary 

1. The browser represents the page using a DOM tree.
2. DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes.
3. You can select element nodes by their id or cl ass attributes, by tag name, or using CSS selector syntax.
4. Whenever a DOM query can return more than one node, it will always return a Node list.
5. From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques.
6. An element node can contain multiple text nodes and child elements that are siblings of each other.
7. In older browsers, implementation of the DOM is inconsistent (and is a popular reason for usingbjQuery).
8. Browsers offer tools for viewing the DOM tree .

