# Images 
>There are many reasons why you might want to add an image to a web page: you might want to include a logo, photograph, illustration, diagram, or chart.
* How to Choosing Images for Your Site
  1. relevent 
  2. Convey Information 
  3. Convey the right mood 
  4. fit the color 

* Storing Images on Your Site 
  > If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses

* Adding Images :
    add this tag to store imge in your page `<img src="" alt="" title=""/>`
    1. src=the path of img 
    2. alt=to provide a text description 
    3. title =additional information 
    4.Height & Width of Images you can use `hight and width ` to specify the hight and width for the image 

* Where to Place Images in Your Code
  1. before a paragraph
  2. inside the start of a paragraph 
  3. in the middle of a paragraph


### Summary 
The <img> element is used to add images to a
web page.
* You must always specify a src attribute to indicate the source of an image and an alt attribute to describe the content of an image.
* You should save images at the size you will be using them on the web page and in the appropriate format.
* Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.


# Color 
> Color can really bring your pages to life.

* Foreground Color `color`
  1. rgb values Values for red, green, and blue are expressed as numbers between `0 and 255`.
  2. hex codes Hex values represent values for red green, and blue in hexadecimal code
  3. color names Colors are represented by predefined names. However, they are very limited in number.


* BackGround Color `background-color`

* CSS 3: Opacity `opacity, rgba `

* CSS 3: HSL Colors 
  > CSS3 introduces an entirely new and intuitive way to specify colors using hue, saturation, and lightness values.

  1. *hue* Hue is the colloquial idea of color. In HSL colors, hue is often represented as a color circle where the angle represents the colornalthough it may also benshown as a slider  with values from 0 to 360.
  2. *saturation* Saturation is the amount of gray in a color. Saturation is represented as a percentage. 100% is full saturation and 0% is a shade of gray.
  3.*lightness* Lightness is the amount of white  (lightness) or black (darkness) in a color. Lightness is represented as a percentage. 0% lightness is black, 100% lightness is white, and 50% lightness is normal. Lightness is sometimesreferred to as luminosity.


### Summary
- Color not only brings your site to life, but also helps
convey the mood and evokes reactions.
- There are three ways to specify colors in CSS:
RGB values, hex codes, and color names.
- Color pickers can help you find the color you want.
- It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).
- CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
- CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.


# Text 
> The properties that allow you to control the appearance of text can be split into two groups:
* Those that directly affect the font and its appearance (including the typeface, whether it is regular, bold or italic, and the size of the text)
* Those that would have the same effect on text no matter what font you were using (including the color of text and the spacing between words and letters)


* Typeface Terminology 
  1. Serif Serif: fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.
  2. Sans-Serif: Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design
  3. Monospace Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)
  4. Weight 1. Light 2. Medium 3. Bold 4. Black
  5.  Style 1. Normal 2. Italic 3. Oblique 
  6.  Stretch 1. Condensed 2. Regular 3. Extended
   
  - When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer.

### Summary
_TEXT_
- There are properties to control the choice of font, size,
weight, style, and spacing.
- There is a limited choice of fonts that you can assume
most people will have installed.
- If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.
- You can control the space between lines of text,
individual letters, and words. Text can also be aligned
to the left, right, center, or justified. It can also be indented.
- You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.


