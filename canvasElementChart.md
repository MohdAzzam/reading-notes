# CHART.JS 
Charts are beeter way to displaying data visually then tables . and there is a lot layout tool . but they’re not always easy to create.

A great way to get started with charts is with `Chart.js`, a JavaScript plugin that uses `HTML5’s canvas` element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

# The `<canvas>` element
`<canvas id="tutorial" width="150" height="150"></canvas>`

At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.

The `id` attribute isn't specific to the `<canvas>` element but is one of the global HTML attributes which can be applied to any HTML element (like class for instance). It is always a good idea to supply an id because this makes it much easier to identify it in a script.

Drawing text 

The canvas rendering context provides two methods to render text:
fillText(text, x, y [, maxWidth])

    Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
strokeText(text, x, y [, maxWidth])

Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

* A fillText example
* A strokeText example


