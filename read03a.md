# Lists

> There are three type of list .

1. Order Lists
2. Bullet lists
3. Definition lists

- Ordered lists are lists where each item in the list is
  numbered. For example, the list might be a set of steps for
  a recipe that must be performed in order, or a legal contract
  where each point needs to be identified by a section
  number.

- Unordered lists are lists that begin with a bullet point
  (rather than characters that indicate order).

- Definition lists are made up of a set of terms along with the
  definitions for each of those terms.

### How we type it in html ?

1. order list `<ol><li></li></ol>` the `li` mean the list iteam
2. unorder list `<ul><li></li></ul>`
3. definition list `<dl><dt> <dd></dd> </dt></dl>` the `dt` mean the tearm the `dd` definition it self

### How we add nested list ?

inside any of li we can added another list `<ol><li></li><li><ol><li></li></ol></li></ol>`

## Summary

- There are three types of HTML lists: ordered,
  unordered, and definition.
- Ordered lists use numbers.
- Unordered lists use bullets.
- Definition lists are used to define terminology.
- Lists can be nested inside one another.

# Boxes

Controlling size of boxes.
Box model for borders, margin and padding.
Displaying and hiding boxes.

- Box Dimensions
  `width, height.`

- we can Limiting Width using
  `min-width, max-width`
- we can Limiting Height using
  `min-height, max-height`

- Overflowing Content
  `hidden, scroll`

- Border, Margin & Padding

  1. Border Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.

  2. Margin Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.

  3. Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents
  4. Whitespace & Vertical Margin The padding and margin properties are very helpful in adding space between various items on the page.

### Summary

1. CSS treats each HTML element as if it has its own box.
2. You can use CSS to control the dimensions of a box.
3. You can also control the borders, margin and padding
   for each box with CSS.
4. It is possible to hide elements using the display and
   visibility properties.
5. Block-level boxes can be made into inline boxes, and
   inline boxes made into block-level boxes.
6. Legibility can be improved by controlling the width of
   boxes containing text and the leading.
7. CSS3 has introduced the ability to create image
   borders and rounded borders.

# DATA TYPES

JavaScript distinguishes between numbers,
strings, and true or false values known as
Booleans.

1. NUMERIC DATA TYPE `15`
2. STRING DATA TYPE `'Hello '`
3. BOOLEAN DATA TYPE `true`

- USING A VARIABLE TO STORE A NUMBER `var number= 99`
- USING A VARIABLE TO STORE A STRING `var userName='Mohammad'`
- USING A VARIABLE TO STORE A BOOLEAN `var isvalid=true `
- CHANGING THE VALUE OF A VARIABLE `var number =100` `number = 500`
- RULES FOR NAMING VARIABLES
  1. The name must begin with a letter, dollar sign ($),or an underscore (\_). It must not start with a number.
  2. The name can contain letters,numbers, dollar sign ($), or an underscore (\_). Note that you must not use a dash(-) or a period (.) in a variable name.
  3. You cannot use keywords or reserved words. Keywords are special words that tell the interpreter to do something. For example, var is a keyword used to declare a variable. Reserved words are ones that may be used in a future version of JavaScript.
  4. case sensitive.
  5. Use a name that describes the kind of information that the variable stores.
  6. If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word.

4. ARRAYS An array is a special type of variable. It doesn't just store one value; it stores a list of values.
   1. You should consider using an array whenever you are working with a list or a set of values that are related to each other.
   2. Arrays are especially helpful
      when you do not know how
      many items a list will contain
      because, when you create the
      array, you do not need to specify
      how many values it will hold.
   3. If you don't know how many
      items a list will contain, rather
      than creating enough variables
      for a long list (when you might
      only use a small percentage
      of them), using an array is
      considered a better solution.

- CREATING AN ARRAY
  You create an array and give it
  a name just like you would any
  other variable (using the var
  keyword followed by the name of
  the array).
  The values are assigned to the
  array inside a pair of square
  brackets, and each value is
  separated by a comma. The
  values in the array do not need
  to be the same data type, so you
  can store a string, a number and
  a Boolean all in the same array.

- VALUES IN ARRAYS Values in an array are accessed as if they are in
  a numbered list. It is important to know that the
  numbering of this list starts at zero (not one).
- ACCESSING & CHANGING VALUES IN AN ARRAY
  `Create the array`
  `var colors = ['white','black' ,'custom'];`
  `II Update the third item in the array`
  `colors[2] = 'beige ' ;`
  `II Get the element with an id of colors`
  `var el = document .getElementByid(' colors') ;`
  `II Replace with third item from the array`
  `el.textContent = colors[2];`

## Loops

> Loops check condition if it's true the block of code will run. Then the condition will be checked again if is still true the code block will work again , it will repeat until the condition become a false

- Type Of Loops : 
  ![typeofloop](https://mohdazzam.github.io/reading-notes/typeofloop.png)

  1. `for(loop counter initialization ;CONDITION_UPDATE){//code}`
  2. `while(CONDITION){//code and COUNTER}`
  3. `do(){//code} while(CONDITION)`

### SWITCH STATEMENTS

> A switch statement starts with a
> variable called the switch value.
> Each case indicates a possible
> value for this variable and the
> code that should run if the
> variable matches that value.

`switch (level) {`
`case 1:`
`msg = 'Good luck on the first test ' ;`
`break;`
`case 2:`
`msg = 'Second of three - keep going!';`
`break;`
`case 3:`
`msg = ' Final round, almost there!';`
`break;`
`default :`
`msg = 'Good l uck!';`
`break;`



### Summary

- if ... else statements allow you to run one set of code
    if a condition is true, and another if it is false.
- switch statements allow you to compare a value
  against possible outcomes (and also provides a default
  option if none match).
- Data types can be coerced from one type to another.
- All values evaluate to either truthy or falsy.
- There are three types of loop: for, while, and
  do ... while. Each repeats a set of statements.
