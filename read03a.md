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

