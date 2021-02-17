# Forms 

Forms are created to collect data from user 
--------------------

### Forms Control
1. adding text
   * Text input
   * Password Input
   * Text Area
2. Making Choices
   * Radio button 
   * check box
   * Drop Down list
3. Submiting Form 
   * Subimt Button 
   * Image Buttton 
4. Uploading File 
   * File Upload 
### How Forms work : 
user fill the data on a form then press to button to submit the information 

#### Form Structure 

`<form  action=""  method="post or get " id="">`
    `<Input type="" name="" id="" />` 
`</form>`


#### Summary 

1. Whenever you want to collect information from visitors you will need a form, which lives inside a `<form>` element.
2. Information from a form is sent in name/value pairs.
3. Each form control is given a name, and the text the user types in or the values of the options they select are sent to the server.
5. HTML5 introduces new form elements which make it easier for visitors to fill in forms.

-------------------------------------------


# Lists, Tables and Forms

1. Bullet Point Styles `list-style-type`
2. Images for Bullets `list-style-image`
3. Positioning the Marker `list-style-position`
4. List Shorthand `list-style`

--------------------------------------------
#### Table Properties
 1. Border on Empty Cells `empty-cells` `show``hide``inheret`
 2. Gaps Between Cells `border-spacing, border-collapse ` `collapse` `separate`

---------------------------------------------
#### Styling Forms
Nobody I know enjoys filling in forms, so if you can make yours look more attractive and easier to use, more people are likely to fill it in. Also, when you come to look at a form in a few different browsers (as shown on the right), you will see that
each browser displays them
differently.
You can Style any element inside the form 
1. Styling Text Inputs
2. Styling Submit Buttons
3. Styling Fieldsets & Legends
4. cursor you can change the mouce cursor inside the form



# Events

The Event will fire up when an action happend on webpage 

-----------------------------------------------
1. UI EVENTS Occur when a user interacts with the browser's user interface (UI) rather than the web page
2. KEYBOARD EVENTS Occur when a user interacts with the keyboard (see also input event)
3. MOUSE EVENTS Occur when a user interacts with a mouse. trackpad, or touchscreen
4. FOCUS EVENTS Occur when an element (e.g., a link or form field) gains or loses focus
5. Form Event Occur when a user interacts with a form element
6. MUTATION EVENTS Occur when the DOM structure has been changed by a script

###  HOW EVENTS TRIGGER JAVASCRIPT CODE
1. selecting element    
2. Indicate which event will trigger (specify event)
3. state the code to run it (call the code) 



## Summary 
1. Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked).
2. Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon.
3. When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user.
4. You can use event delegation to monitor for events that happen on all of the children of an element.
5. The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events.