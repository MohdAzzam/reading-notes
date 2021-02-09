# Links

Tody you will learn abot How to 
1. Creating links between pages
2. Linking to other sites
3. Email links

>Links are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of browsing or surfing.

### Writing Links

How to write a link ?
Links are created using the `<a>` element. Users can click on anything
between the opening `<a>` tag and the closing `</a>` tag. You specify
which page you want to link to using the href attribute.

`<a href="">Name</a> `

you can link any thing you want pages another website divs on the same page 

* Email Links  
 mailto: email-links.html HTML To create a link that starts up the user's email program and addresses an email to a specified email address, you use the <a> element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to.
 >this is the way to write it 
 `<a href="mailto:jon@example.org">Email Jon</a>`

How to open link in new tap ?
you can do this using `_blank` inside `target` 
`<a href="http://www.imdb.com" target="_blank">` 

How to Linking to a Specific Part of the Same Page?
inide the div or any html element add `id` and link it using that id 
`<p id ="top">blbalabbalba</p>`
`<a href="#top">` 

### Summary
Links are created using the <a> element.
* The <a> element uses the href attribute to indicate
the page you are linking to.
* If you are linking to a page within your own site, it is
best to use relative links rather than qualified URLs.
* You can create links to open email programs with an
email address in the "to" field.
* You can use the id attribute to target elements within
a page that can be linked to.



# Layout 

* Controlling the position of elements 
* Creating site layouts
* Designing for different sized screens
  

Key Concepts in Positioning Elements
* Building Blocks
CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.
Block-level boxes start on a new line and act as the main building blocks
of any layout, while inline boxes flow between surrounding text. You can
control how much space each box takes up by setting the width of the
boxes (and sometimes the height, too). To separate boxes, you can use
borders, margins, padding, and background colors.

1. Block-level elements start on a new line Examples include:
`<h1> <p> <ul> <li>`
2. Inline elements flow in between surrounding text Examples include:
<img> <b> <i>


* Containing Elements
  If one block-level element sits inside another
  block-level element then the outer box is
  known as the containing or parent element.
  It is common to group a number of elements together inside a <div>
  (or other block-level) element. For example, you might group together
  all of the elements that form the header of a site (such as the logo and
  the main navigation). The <div> element that contains this group of
  elements is then referred to as the containing element.

* Controlling the Position of Elements
  CSS has the following positioning schemes that allow you to control
    the layout of a page: normal flow, relative positioning, and absolute
    positioning. You specify the positioning scheme using the position
    property in CSS. You can also float elements using the float property.
    1. Normal flow Every block-level element
    appears on a new line, causing
    each item to appear lower down
    the page than the previous one.
    Even if you specify the width
    of the boxes and there is space
    for two elements to sit side-byside,
    they will not appear next
    to each other. This is the default
    behavior (unless you tell the
    browser to do something else).`
    2. Relative Positioning
        This moves an element from the
        position it would be in normal
        flow, shifting it to the top, right,
        bottom, or left of where it
        would have been placed. This
        does not affect the position of
        surrounding elements; they stay
        in the position they would be in
        in normal flow.
    3. Absolute positioning
        This positions the element
        in relation to its containing
        element. It is taken out of
        normal flow, meaning that it
        does not affect the position
        of any surrounding elements
        (as they simply ignore the
        space it would have taken up).
        Absolutely positioned elements
        move as users scroll up and
        down the page.

To indicate where a box should be positioned, you may also need to use
box offset properties to tell the browser how far from the top or bottom
and left or right it should be placed. (You will meet these when we
introduce the positioning schemes on the following pages.)
*Fixed Positioning*
    This is a form of absolute
    positioning that positions
    the element in relation to the
    browser window, as opposed
    to the containing element.
    Elements with fixed positioning
    do not affect the position of
    surrounding elements and they
    do not move when the user
    scrolls up or down the page.

*Floating Elements*
    Floating an element allows
    you to take that element out
    of normal flow and position
    it to the far left or right of a
    containing box. The floated
    element becomes a block-level
    element around which other
    content can flow.

When you move any element from normal flow, boxes can overlap. The `z-index` property allows you to control which box appears on top.

* Normal Flow `position:static`
* Relative Positioning `position:relative`
* Absolute Positioning `position:absolute`
* Fixed Positioning `position:fixed`
* Overlapping Elements `z-index`
* Floating Elements `float`
* Clearing Floats  `clear`

### Screen Sizes
Different visitors to your site will have different sized screens that show
different amounts of information, so your design needs to be able to
work on a range of different sized screens.

Screen Resolution
> Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.

Page Sizes
> Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).

## Summary 

- <div> elements are often used as containing elements
to group together sections of a page.
- Browsers display pages in normal flow unless you
specify relative, absolute, or fixed positioning.
- The float property moves content to the left or right
of the page and can be used to create multi-column
layouts. (Floated items require a defined width.)
- Pages can be fixed width or liquid (stretchy) layouts.
- Designers keep pages within 960-1000 pixels wide,
and indicate what the site is about within the top 600
pixels (to demonstrate its relevance without scrolling).
- Grids help create professional and flexible designs.
- CSS Frameworks provide rules for common tasks.
- You can include multiple CSS files in one page.


# Functions, Methods, and Objects 
>Browsers require very detailed instructions about what we want them to do. Therefore, complex scripts can run to hundreds (even thousands) of lines. Programmers use functions, methods, and objects to organize their code. This chapter is divided into three sections that introduce:
1. Functions : Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of st atements).
`function nameofit(param){`
 `   //code`
`}`

calling the function `nameofit()`


How does pair programming work?
While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

Why pair program?
While learning to code, developers likely study several programming languages. Similar to a foreign language class, there are four fundamental skills that help anyone learn a new language: Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea Reading: understanding what written language intends to convey Writing: producing from scratch a meaningful

Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.

During a five-hour paired lab session, Code Fellows students work on all four of these language-specific skills. The abilities they foster will serve them well in completing assignments, in their own communication and learning, in interviews, and in readiness for a job at a company that utilizes this agile practice.

Wow, all that? Let’s take a look!

1. Greater efficiency
It is a common misconception that pair programming takes a lot longer and is less efficient. In reality, when two people focus on the same code base, it is easier to catch mistakes in the making. Research indicates that pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging (let alone exposing users to a broken product). So, in the long-run, it’s often actually more efficient than two people working on separate features. When coming up with ideas and discussing solutions out loud, two programmers may come to a solution faster than one programmer on their own. Also, when the pair is stuck, both programmers can research the problem and reach a solution faster. Researches also identified pairing enhances technical skills, team communication, and even enjoyability of coding in the workplace.

2. Engaged collaboration
When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone. It is harder to procrastinate or get off track when someone else is relying on you to complete the work. Popping open your Facebook timeline is just that less enticing when someone else is looking at your screen.

Another important aspect of learning to program is knowing when to ask for help. We advise our students to spend no more than fifteen minutes stuck on a problem before asking a teaching assistant or instructor for help. When developers pair program, they rely more on each other and can often find a solution together without needing to ask for additional help. Ultimately, this boosts overall confidence.

3. Learning from fellow students
Everyone has a different approach to problem solving; working with a teammate can expose developers to techniques they otherwise would not have thought of. If one developer has a unique approach to a specific problem, pair programming exposes the other developer to a new solution.

Often times, the developers in a pairing have different skill sets. If one programmer is more experienced in a certain skill, they can teach a student who is less familiar with that area. The less experienced developer benefits from the experienced developer’s knowledge and guidance, and the latter benefits from explaining the topic in their own words, further solidifying their own understanding.

4. Social skills
Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key. This can become more difficult when two programmers have different personalities. Pair programming not only improves programming skills, but can also help programmers develop their interpersonal skills. When just grabbing the keyboard and taking over isn’t an option, getting good at finding the right words is a skill unto itself.

This has long-term career impacts. As much as employers want strong programmers, they know it’s essential to hire people who can work well with others.

5. Job interview readiness
A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen. They will carry out exercises together, such as code challenges, building a project or feature, or debugging an existing code base. By doing so, companies can get a better feel for how an applicant will fit into the team and their collaboration style.

For most roles, the ability to work with and learn from others and stellar communication skills are as (or more!) important to a company than specific technical skills. Pair programming strengthens all of those skills.

6. Work environment readiness
Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.

