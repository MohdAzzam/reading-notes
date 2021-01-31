# Introducing CSS


> * What CSS does
  * How CSS works
  * Rules, properties, and values


`CSS` allows you to create rules that specify how the content of
an element should appear. For example, you can specify that
the background of the page is cream, all paragraphs should
appear in gray using the Arial typeface, or that all level one
headings should be in a blue, italic, Times typeface.

## Understanding CSS:

###### Thinking Inside the Box
> The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element.



### BLOCK & INLINE ELEMENTS
> Block level elements look like they start on a new line. Examples include the `<h1>-<h6>, <p> and <div>` elements.
> Inline elements flow within the text and do not start on a new line. Examples include `<b>, <i>,<img>, <em> and <span>`.


CSS allows you to create rules that control the
way that each individual box (and the contents
of that box) is presented.

Example Styles
| Boxes       | Text        | Specific    |
| ----------- | ----------- | ----------- |
| Width and height Borders (color, width, and style) Background color and images Position in the browser window | Typeface Size ColorItalics, bold, uppercase,lowercase, small-caps       |   There are also specific ways in which you can style certain elements such as lists, tables, and forms.      |


###### CSS Associates Style rules with HTML elements
>  CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule          contains two parts: a s`elector and a declaration`.


![css](https://mohdazzam.github.io/-reading-notes/css.png)



> There are three way to add css to Html 

* Inline inside  the element `<h1 style="color:blue;"> </h1>` 
* External adding dierctory `style.css` and connected it using `<link src="">`
* Internal inside HTML page between `<style></style>`


#### Selectors 

![css](https://mohdazzam.github.io/-reading-notes/selector.png)

# Summary

> CSS treats each HTML e XX lement as if it appears inside
its own box and uses rules to indicate how that
element should look.
> Rules are made up of selectors (that specify the
elements the rule applies to) and declarations (that
indicate what these elements should look like).
> Different types of selectors allow you to target your
rules at different elements.
> Declarations are made up of two parts: the properties
of the element that you want to change, and the values
of those properties. For example, the font-family
property sets the choice of font, and the value arial
specifies Arial as the preferred typeface.
> CSS rules usually appear in a separate document,
although they may appear within an HTML page.

# Questions

* What is CSS?


* Cite different types of CSS ?

* How to use CSS selector? 






