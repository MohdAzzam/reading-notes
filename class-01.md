# Introduction

### How People Access the Web

 `Web Servers`
: People access websites using software called a web browser. Popular examples include Firefox, Internet Explorer, Safari, Chrome, and Opera.
 In order to view a web page,
 users might type a web address
 into their browser, follow a
 link from another site, or use a
 bookmark.

 `Web Servers` 
 : When you ask your browser for a web page, the request is sent across the Internet to a special computer known as a web server which  hosts the website.
 `Devices`
 : People are accessing websites
 on an increasing range of devices
 including desktop computers,
 laptops, tablets, and mobile
 phones. It is important to
 remember that various devices
 have different screen sizes and
 some have faster connections to
 the web than others.

 `Screen readers`
 : Screen readers are programs
 that read out the contents of a
 computer screen to a user. They
 are commonly used by people
 with visual impairments.


### How Websites Are Created
> All websites use HTML and CSS, but content
management systems, blogging software, and
e-commerce platforms often add a few more
technologies into the mix.
 


### How the Web Works ?

 When you visit a website, the web server
    hosting that site could be anywhere in the
    world. In order for you to find the location of
    the web server, your browser will first connect
    to a Domain Name System (DNS) server

1. When you connect to the web,
you do so via an Internet Service
Provider (ISP). You type a
domain name or web address
into your browser to visit a site;
for example: google.com,
bbc.co.uk, microsoft.com.
2. Your computer contacts a
network of servers called
Domain Name System (DNS)
servers. These act like phone
books; they tell your computer
the IP address associated with
the requested domain name.
An IP address is a number
of up to 12 digits separated
by periods / full stops. Every
device connected to the web
has a unique IP address; it is
like the phone number for that
computer.
3. The unique number that the
DNS server returns to your
computer allows your browser
to contact the web server
that hosts the website you
requested. A web server is a
computer that is constantly
connected to the web, and is set
up especially to send web pages
to users.



# HTML Introduction 
 HTML is the standard markup language for creating Web pages. 


#### What is HTML?
* HTML stands for Hyper Text Markup Language
* HTML is the standard markup language for creating Web pages
* HTML describes the structure of a Web page
* HTML consists of a series of elements
* HTML elements tell the browser how to display the content
* HTML elements label pieces of content such as "this is a heading", "this is a paragraph", "this is a link", etc.

###### HTML Describes the Structure of Pages

`<html>`
`<body>`
`<h1>This is the Main Heading</h1>`
`<p>This text might be an introduction to the rest of
the page. And if the page is a long one it might
be split up into several sub-headings.<p>`
`<h2>This is a Sub-Heading</h2>`
`<p>Many long articles have sub-headings so to help
you follow the structure of what is being written.
There may even be sub-sub-headings (or lower-level
headings).</p>`
`<h2>Another Sub-Heading</h2>`
`<p>Here you can see another sub-heading.</p>`
`</body>`
`</html>`

The `<html> `element is the root element of an HTML page
The `<head>` element contains meta information about the HTML page
The `<title>` element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
The `<body>` element defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
The `<h1>` element defines a large heading
The `<p>` element defines a paragraph

### What is an HTML Element?
An HTML element is defined by a start tag, some content, and an end tag:
the HTML element is everything from the start tag to the end tag:
`<h1>My First Heading</h1>`

| Start tag | Element content  | End tag |
| --------- | ---------------- | ------- |
| `<h1>	`   | My First Heading | `</h1>` |



##### Creating a Web Page on a PC

1. To create your first web page on
a PC, start up Notepad.
2. Type the html code
3. save the file with extension `.html`
4. close the file
5. click agin on the file it will open the html page with your default browser 
   

### Summary
* HTML pages are text documents.
* HTML uses tags (characters that sit inside angled
brackets) to give the information they surround special
meaning.
* Tags are often referred to as elements.
* Tags usually come in pairs. The opening tag denotes
the start of a piece of content; the closing tag denotes
the end.
* Opening tags can carry attributes, which tell us more
about the content of that element.
* Attributes require a name and a value.
* To learn HTML you need to know what tags are
available for you to use, what they do, and where they
can go.




# Extra Markup
1. DOCTYPEs `<!DOCTYPE  >`
2. Comments in HTML  `<!-- -->`
3. ID Attribute. `<p id="">`
4. Class Attribute. `<p class="">`
5. Block Elements `<p>`
6. Inline Elements `<img>`
7. Grouping Text & Elements In a Block `<div>`
8. Grouping Text & Elements Inline `<span>`
9. IFrames `<ifram>`
10. Information About Your Pages `<meta>`

### Summary EXTRA MARKUP
* DOCTYPES tell browsers which version of HTML you
are using.
*  You can add comments to your code between the
<!-- and --> markers.
*  The id and class attributes allow you to identify
particular elements.
*  The <div> and <span> elements allow you to group
block-level and inline elements together.
*  <iframes> cut windows into your web pages through
which other pages can be displayed.
*  The <meta> tag allows you to supply all kinds of
information about your web page.
*  Escape characters are used to include special
characters in your pages such as <, >, and ©.



# HTML5
HTML5 is a markup language used for structuring and presenting content on the World Wide Web. It is the fifth and last major HTML version that is a World Wide Web Consortium (W3C) recommendation. The current specification is known as the HTML Living Standard. It is maintained by a consortium of the major browser vendors (Apple, Google, Mozilla, and Microsoft), the Web Hypertext Application Technology Working Group (WHATWG).

> HTML5 was first released in a public-facing form on 22 January 2008,
 with a major update and "W3C Recommendation" status in October 2014. Its goals were to improve the language with support for the latest multimedia and other new features; to keep the language both easily readable by humans and consistently understood by computers and devices such as web browsers, parsers, etc., without XHTML's rigidity; and to remain backward-compatible with older software. HTML5 is intended to subsume not only HTML 4 but also XHTML 1 and DOM Level 2 HTML.

HTML5 includes detailed processing models to encourage more interoperable implementations; it extends, improves, and rationalizes the markup available for documents and introduces markup and application programming interfaces (APIs) for complex web applications. For the same reasons, HTML5 is also a candidate for cross-platform mobile applications because it includes features designed with low-powered devices in mind.

Many new syntactic features are included. To natively include and handle multimedia and graphical content, the new `<video>`, `<audio>` and `<canvas>` elements were added, and support for scalable vector graphics (SVG) content and MathML for mathematical formulas was also added. To enrich the semantic content of documents, new page structure elements such as `<main>`, `<section>`, `<article>`, `<header>`, `<footer>`, `<aside>`, `<nav>`, and `<figure>` are added. New attributes were introduced, some elements and attributes were removed, and others such as `<a>`, `<cite>`, and `<menu>` were changed, redefined, or standardized. The APIs and Document Object Model (DOM) are now fundamental parts of the HTML5 specification, and HTML5 also better defines the processing for any invalid documents


# Process & Design

1. Who is the Site For? Every website should be designed for the
target audience—not just for yourself or the
site owner. It is therefore very important to
understand who your target audience is.
2. Why People Visit YOUR Website Now that you know who your visitors are, you
need to consider why they are coming. While
some people will simply chance across your
website, most will visit for a specific reason.
3. What Your Visitors are Trying to Achieve It is unlikely that you will be able to list every
reason why someone visits your site but you
are looking for key tasks and motivations. This
information can help guide your site designs.
4. What Information Your Visitors Need You know who is coming to your site and why
they are coming, so now you need to work out
what information they need in order to achieve
their goals quickly and effectively.
5. How Of ten People WillVisit Your Site Some sites benefit from being updated more
frequently than others. Some information (such
as news) may be constantly changing, while
other content remains relatively static.
6. Site Maps Now that you know what needs to appear
on your site, you can start to organize the
information into sections or pages. 
![sitemap](https://mohdazzam.github.io/reading-notes/sitemap.png)


7. WireFrames A wireframe is a simple sketch of the key
information that needs to go on each page of a
site. It shows the hierarchy of the information
and how much space it might require.
8. Getting your message across using design The primary aim of any kind of visual design
is to communicate. Organizing and prioritizing
information on a page helps users understand
its importance and what order to read it in.
9. Visual hierarchy Most web users do not read entire pages. Rather, they skim to find
information. You can use contrast to create a visual hierarchy that gets
across your key message and helps users find what they are looking for 1. size 1. color 1. style 

10. grouping and Similarity When making sense of a design, we tend to organize visual elements
into groups. Grouping related pieces of information together can make a
design easier to comprehend. Here are some ways this can be achieved.
11. Designing Navigation Site navigation not only helps people find where they want to go, but also
helps them understand what your site is about and how it is organized.
Good navigation tends to follow these principles... 1. Concise 2. Clear 3. Selective



# ABC Of programing 
![sitemap](https://mohdazzam.github.io/reading-notes/abc.png)
