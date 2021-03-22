# jQuery

Write Less Do more 
>jQuery is a JS library and it offers a simple way to achieve a variety of common JavaScript tasks quickly and consistently, across all major browsers and without any fallback code needed.

----------------------------

## jQuery used for

1. Finding element using css selectors, id element, class elememnt   `$('li.hot')`
2. Do something with element using jQuery `$('li.hot').addClass('az');`

---------------------

## jQuery methods that get and set 

jQuery store referenecs to elements 

`let content = $('li').html()` get the data
`let content = $('li').html('Change')` set the data

-----------------------------

## check the page is Ready to work 

the best practises to start jQuery code after the html content is render on the page 
so this is how to wait the html code render then start the jQuery 
`$(document).ready(function(){//Code gose here })`
or we use the short way 
`$(function (){//code Gose here })`

------------------------

### Updating element 

1. . html() if we print this out and was inside the selector another html element it will show in the console
2. .text() print out just the text
3. .replaceWith() replace the selected element content with new content
4. . remove() remove the elemnt 

-------------------

### INSERTING ELEMENTS

1. .before() insert the content befor the selected element
2. .after() insert the content after the selected element
3. .prepend() insert the content inside the selected element after opining tag
4. .append() insert the content inside the selected element befor opining tag
`.befor()<li>.prepend()items .append()</li>.after()`

-------------------

### GETTING AND SETTING ATTRIBUTE VALUES

1. attr() get or sett attr and his val 
2. removeAttr() remove any selectedAttr value 
3. .addClass() adding new class 
4. removeClass() remove class 

--------------------

### Event Method 

The • on () method is used to handle all events.




### Ways to include jquery in your page 

1. using CDN 
2. download the file and import it in the js file 





---------------------------------------


# 6 Reasons for Pair Programming

Iterative loops. Code reviews. Fast feedback. Error checking and linting. These are software engineering practices that have proven to dramatically improve the quality of code developers produce. What if you can could get all of this, instantaneously, while typing code line by line and character by character? You can, with pair programming, a technique common to many agile work environments.

More “two heads are better than one” than “stop reading over my shoulder,” pair programming is the practice of two developers sharing a single workstation to interactively tackle a coding task together.

-----------------------

#### How does pair programming work? 

The Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

#### Why pair program?

While learning to code, developers likely study several programming languages. Similar to a foreign language class, there are four fundamental skills that help anyone learn a new language: Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea Reading: understanding what written language intends to convey Writing: producing from scratch a meaningful

Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.

1. Greater efficiency 
2. Engaged collaboration
3. Learning from fellow students
4. Job interview readiness
5. Work environment readiness