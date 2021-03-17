# RESPONSIVE WEB DESIGN and FLOATS

----------------------------------------

> The Internet took off quicker than anyone would have predicted, growing like crazy. Now, for the past few years, mobile growth has exploded onto the scene. The growth of mobile Internet usage is also far out pacing that of general Internet usage growth
> With the growth in mobile Internet usage comes the question of how to build websites suitable for all users. The industry response to this question has become responsive web design, also known as RWD.

-------------------------------------------------------------;

## Responsive Overview

Practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.

--------------------------------------------------------;

### Responsive vs. Adaptive vs. Mobile

Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation, such as change.

Mobile, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users.

__Flexible Layouts__
Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media. The first part, flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. Flexible grids are built using relative length units, most commonly percentages or `em` units. These relative lengths are then used to declare common grid property values such as `width`, `margin`, or `padding`.

Flexible layouts do not advocate the use of fixed measurement units, such as pixels or inches. Reason being, the viewport height and width continually change from device to device. Website layouts need to adapt to this change and fixed values have too many constraints. Fortunately, Ethan pointed out an easy formula to help identify the proportions of a flexible layout using relative values.

`target ÷ context = result`
The formula is based around taking the target width of an element and dividing it by the width of it’s parent element. The result is the relative width of the target element.

__Media Queries__
Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation.

__Mobile First__
One popular technique with using media queries is called mobile first. The mobile first approach includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.

__Flexible Media__
The final, equally important aspect to responsive web design involves flexible media. As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.

-----------------------------------------------------------;

## All About Floats

Float is a CSS positioning property. To understand its purpose and origin, we can look to print design. In a print layout, images may be set into the page such that text wraps around them as needed. This is commonly and appropriately called “text wrap”.

Floats can be used to create entire web layouts.

__Clearing the Float__
Float’s sister property is `clear`. An element that has the `clear` property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float.
