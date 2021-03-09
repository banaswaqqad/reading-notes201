# Forms 

### Form Controls : 

**There are several types of form controls that you can use to collect information from visitors to your site.**
1. ADDING TEXT:
2. Making Choices:
3. Submitting Forms

### How Forms Work ? 
**steps** : 
1. A user fills in a form and then presses a button 
to submit the information to the server.
2. The name of each form 
control is sent to the 
server along with the 
value the user enters or 
selects.
3. The server processes 
the information using a 
programming language 
such as PHP, C#, VB.net, 
or Java. It may also store 
the information in a 
database.
4. The server creates a new 
page to send back to the 
browser based on the 
information received.

**To differentiate between various pieces of inputted data, information is sent from the browser to the server using name/value pairs**

## Form Structure : 

1. `<form>` : 

Form controls live inside a 
`<form>` element. This element 
should always carry the action
attribute and will usually have a 
method and id attribute too.

* action
Every `<form>` element requires 
an action attribute. Its value
is the URL for the page on the 
server that will receive the 
information in the form when it 
is submitted.

* method
Forms can be sent using one of 
two methods: get or post.

With the get method, the values 
from the form are added to 
the end of the URL specified in 
the action attribute. The get
method is ideal for:
* short forms (such as search 
boxes)
* when you are just retrieving 
data from the web server 
(not sending information that 
should be added to or deleted 
from a database)

2. text input :

`<input>`
The `<input>` element is used 
to create several different form 
controls. 
The value of the type
attribute determines what kind 
of input they will be creating.
type="text"

When the type attribute has a 
value of text, it creates a single￾line text input.

* name
When users enter information 
into a form, the server needs to 
know which form control each 
piece of data was entered into. 
(For example, in a login form, the 
server needs to know what has 
been entered as the username 
and what has been given as the 
password.) Therefore, each form 
control requires a name attribute. 
The value of this attribute 
identifies the form control and is 
sent along with the information 
they enter to the server. 

* maxlength
You can use the maxlength
attribute to limit the number 
of characters a user may enter 
into the text field. Its value is the 
number of characters they may 
enter

* size
The size attribute should not 
be used on new forms. It was 
used in older forms to indicate 
the width of the text input 
(measured by the number of 
characters that would be seen


3. Password Input : 
`<input>`

type="password"
When the type attribute has 
a value of password it creates 
a text box that acts just like a 
single-line text input, except 
the characters are blocked out. 
They are hidden in this way so 
that if someone is looking over 
the user's shoulder, they cannot 
see sensitive data such as 
passwords.

* name
The name attribute indicates 
the name of the password input, 
which is sent to the server with 
the password the user enters.
size, maxlength
It can also carry the size and 
* maxlength attributes like the 
the single-line text input

4. textarea

The `<textarea>` element 
is used to create a mutli-line 
text input. Unlike other input 
elements this is not an empty 
element. It should therefore have 
an opening and a closing tag. 
Any text that appears between 
the opening `<textarea>` and 
closing `</textarea>` tags will 
appear in the text box when the 
page loads.
If the user does not delete any 
text between these tags, this 
message will get sent to the 
server along with whatever the 
user has typed. (Some sites 
use JavaScript to clear this 
information when the user clicks 
in the text area.)

5. Radio Button : 

<input>

type="radio"

Radio buttons allow users to pick 
just one of a number of options.

* name
The name attribute is sent to 
the server with the value of the 
option the user selects. 

* value
The value attribute indicates 
the value that is sent to the 
server for the selected option. 
The value of each of the buttons 
in a group should be different 
(so that the server knows which 
option the user has selected).

* checked
The checked attribute can be 
used to indicate which value (if 
any) should be selected when 
the page loads. The value of this 
attribute is checked. Only one 
radio button in a group should 
use this attribute.

6. Drop Down List Box : 

`<select>`
A drop down list box (also 
known as a select box) allows 
users to select one option from a 
drop down list.

The <select> element is used 
to create a drop down list box. It 
contains two or more `<option>`
elements. 

* name
The name attribute indicates the 
name of the form control being 
sent to the server, along with the 
value the user selected.

* `<option>`
The `<option>` element is used 
to specify the options that the 
user can select from. 

* value
The `<option>` element uses the 
value attribute to indicate the 
value that is sent to the server 
along with the name of the 
control if this option is selected.


* selected
The selected attribute can be 
used to indicate the option that 
should be selected when the 
page loads. The value of this 
attribute should be selected

7. Submit button : 

`<input>`
type="submit"
The submit button is used to 
send a form to the server.
* name
It can use a name attribute but it 
does not need to have one.
* value
The value attribute is used to 
control the text that appears 
on a button. It is a good idea to 
specify the words you want to 
appear on a button because the 
default value of buttons on some 
browsers is ‘Submit query’ and 
this might not be appropriate for 
all kinds of form.

8. Button & hidden Controls :

`<button>`
The `<button>` element was 
introduced to allow users more 
control over how their buttons 
appear, and to allow other 
elements to appear inside the 
button.

* type="hidden"
 some form which type = hidden  
are not shown on the 
page (although you can see them 
if you use the View Source option 
in the browser).

9. Grouping Form Elements :

`<fieldset>`
You can group related form 
controls together inside the 
`<fieldset>` element. This is 
particularly helpful for longer 
forms.
Most browsers will show the 
fieldset with a line around 
the edge to show how they are 
related. The appearance of these 
lines can be adjusted using CSS.
`<legend>`
The `<legend>` element can 
come directly after the opening 
`<fieldset>` tag and contains a 
caption which helps identify the 
purpose of that group of form 
controls.


## HTML5:
1. #### Form Validation 
Validation helps ensure the 
user enters information in a 
form that the server will be able 
to understand when the form 
is submitted.
2. #### HTML5: Date input : 
`<input>`
Many forms need to gather 
information such as dates, email 
addresses, and URLs. This has 
traditionally been done using 
text inputs.
HTML5 introduces new form 
controls to standardize the 
way that some information is 
gathered. Older browsers that 
do not recognize these inputs 
will just treat them as a single 
line text box. 
* type="date"
If you are asking the user for a 
date, you can use an `<input>`
element and give the type
attribute a value of date. 
This will create a date input in 
browsers that support the new 
HMTL5 input types. 
3. #### Email & URL Input :

`<input>`
HTML5 has also introduced 
inputs that allow visitors to 
enter email addresses and URLs. 
Browsers that do not support 
these input types will just treat 
them as text boxes.
type="email"
If you ask a user for an email 
address, you can use the email 
input. Browsers that support 
HTML5 validation will check 
that the user has provided 
information in the correct format 
of an email address. Some smart 
phones also optimize their 
keyboard to display the keys you 
are most likely to need when 
entering an email address (such 
as the @ symbol).

type="url"
A URL input can be used when 
you are asking a user for a web 
page address. Browsers that 
support HTML5 validation will 
check that the user has provided 
information in the format of 
a URL. Some smart phones 
also optimize their keyboard to 
display the keys you are most 
likely to need when entering a 
URL.

4. Search input 
`<input>`
If you want to create a single 
line text box for search queries, 
HTML5 provides a special type 
of input for that purpose.
* type="search" :
If you want to create a single 
line text box for search queries, 
HTML5 provides a special 
search input.
* placeholder
On any text input, you can 
also use an attribute called 
placeholder whose value is 
text that will be shown in the 
text box until the user clicks in 
that area. Older browsers simply 
ignore this attribute.



# Lists, Tables and Forms 

 **Bullet point styles** : 
  list-style-type 

The list-style-type property 
allows you to control the shape 
or style of a bullet point (also 
known as a marker). 
It can be used on rules that 
apply to the `<ol>`, `<ul>`, and `<li>`
elements.

**Images for bullets**
You can specify an image to act 
as a bullet point using the
list-style-image property 


**Table properties** : 
1. width to set the width of the 
table
2. padding to set the space 
between the border of each table 
cell and its content
3. text-transform to convert the 
content of the table headers to 
 uppercase
4. letter-spacing, font-size
to add additional styling to the 
content of the table headers
5. border-top, border-bottom
to set borders above and below 
 the table headers
6. text-align to align the writing 
to the left of some table cells and 
to the right of the others
7. background-color to change 
the background color of the 
alternating table rows
8. :hover to highlight a table row 
when a user's mouse goes over it


## Styling Text input : 

* font-size sets the size of the 
text entered by the user.
color sets the text color, and 
background-color sets the 
background color of the input.

* border adds a border around 
the edge of the input box, and
border-radius can be used 
to create rounded corners (for 
browsers that support this 
property).

* The :focus pseudo-class is 
used to change the background 
color of the text input when it 
is being used, and the :hover
psuedo-class applies the same 
styles when the user hovers over 
them.

* background-image adds a 
background image to the box. 
Because there is a different 
image for each input, we are 
using an attribute selector 
looking for the value of the id
attribute on each input.

## styling submit buttons 

## Styling Fieldsets& Legends


###  Aligning Form Controls: Problem 
Labels for form elements are 
often different lengths, which 
means that the form controls will 
not appear in a straight line

#### Aligning Form Controls: Solution
Each row of the form has a title 
telling users what they need to 
enter. For the text inputs, the 
title is in the `<label>` element. 
For the radio buttons, the title is 
in a `<span>` element. Both have 
a class attribute with a value of 
title. 
We can use a property called 
float to move the titles to the 
left of the page 

By setting the width property 
on those elements, we know that 
the titles will each take up the 
same width. Therefore, the form 
controls next to them will line up.


### Cursor styles : 
The cursor property allows 
you to control the type of mouse 
cursor that should be displayed 
to users.


# EVENT 



## HOW EVENTS TRIGGER  JAVASCRIPT CODE
1.  
Select t he element 
node(s) you want the 
script to respond to

2. 
Indicate which event on 
the selected node(s) will 
trigger the response.

3. 
State the code you want 
to run when the event 
occurs. 
When the event occurs, on a 
specified element, it will trigger 
a function. This may be a named 
or an anonymous function. 

### THREE WAYS TO BIND AN EVENT TO AN ELEMENT

**There are three types of event handlers** 
1. HTML EVENT HANDLERS :
This is bad practice, but you 
need to be aware of it because 
you may see it in older code
2. TRADITIONAL DOM EVENT HANDLERS 
DOM event handlers were 
introduced in the original 
specification for the DOM. 
They are considered better than 
HTML event handlers because 
they let you separate the 
JavaScript from the HTML. 
3. DOM LEVEL 2 EVENT LISTENERS 
Event listeners were introduced 
in an update to the DOM 
specification (DOM level 2, 
released in the year 2000). 
They are now the favored way of 
handling events. 

## SUPPORTING OLDER VERSIONS OF IE 
ES-8 had a different event model and did not support 
addEventL i stener() but you can provide fallback code 
to make event listeners work with older versions of IE. 

## event flow 
**what is Event bubbling and capturing**
Event bubbling and capturing are two ways of event propagation in the HTML DOM API, when an event occurs in an element inside another element, and both elements have registered a handle for that event. The event propagation mode determines in which order the elements receive the event.

With bubbling, the event is first captured and handled by the innermost element and then propagated to outer elements.

With capturing, the event is first captured by the outermost element and propagated to the inner elements.

Capturing is also called "trickling", which helps remember the propagation order:

trickle down, bubble up

Back in the old days, Netscape advocated event capturing, while Microsoft promoted event bubbling. Both are part of the W3C Document Object Model Events standard (2000).


We can use the addEventListener(type, listener, useCapture) to register event handlers for in either bubbling (default) or capturing mode. To use the capturing model pass the third argument as true.


## THE EVENT OBJECT 
When an event occurs, the event object tells 
you information about the event, and the 
element it happened upon.

## EVENT DELEGATION 
Creating event listeners for a lot of elements 
can slow down a page, but event flow allows 
you to listen for an event on a parent element.

## CHANGING DEFAULT BEHAVIOR 
The event object has methods that change: 
the default behavior of an element and how 
the element's ancestors respond to the event

## DIFFERENT EVENT TYPES 

 1. UI EVENTS : 
  Occur when a user interacts with the browser's user interface (UI) rather than the web page 
  
 ex : error , resize ... etc 

 2. KEYBOARD EVENTS :
  Occur when a user interacts with the keyboard (see also input event) 
  
 3. MOUSE EVENTS:
  Occur when a user interacts with a mouse. trackpad, or touchscreen
  ex : click , dbl click ,mousemove ... etc 
 4. FOCUS EVENTS: 
   Occur when an element (e.g., a link or form field) gains or loses focus
   ex : focus / focus in 
       blur / focusout 
 
 5. FORM EVENTS  
 Occur when a user interacts with a form element 
 ex : input ,change,submit ...etc  
 6. MUTATION EVENTS*
 Occur when the DOM structure has been changed by a script 
 ex : DOMSubtreeModified ,DOMNodelnserted, DOMNodeRemoved 