# Understanding The Problem Domain  

they said that Understanding The Problem Domain is The Hardest Part Of Programming 

### Why problem domains are hard ?
Writing code is a lot like putting together the puzzle's peaces .  We put together code with the purpose of building components that we have taken out of the “bigger picture” of the problem domain.

The big issue is that many problem domains are like a puzzle with a blurry picture or no picture at all.

**Programming is easy if you understand the problem domain**

The more and more I write code, the more I learn that understanding the problem is the most critical piece to the equation.
 It is very difficult to solve a problem before you know the question. 
  It’s like buzzing in on Jeopardy before you hear the clue and shouting out random questions.

### What can you do about it?
If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

1. Make the problem domain easier
2. Get better at understanding the problem domain

**You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.**

What I mean by this is that it is often beneficial to take a part of the problem and fully understand that part before expanding the problem domain.


# WHAT IS AN OBJECT? 

Objects group together a set of variables and functions to create a model 
of a something you would recognize from the real world. In an object, 
variables and functions take on new names.

Like variables and named functions, 
properties and methods have a 
name and a value. **In an object**, 
that name is called a key. 
An object cannot have two keys 
with the same name. This is 
because keys are used to access 
their corresponding values. 
The value of a property can be a 
string, number, Boolean, array, or 
even another object. The value of a 
method is always a function. 

## creating an object : 

1. literal notation 

ex : assume we have  Object is called hotel which 
represents a hotel called Quay 
with 40 rooms (25 of which have 
been booked). 
Next, the content of the page 
is updated with data from this 
object. It shows the name of the 
hotel by accessing the object's 
name property and the number 
of vacant rooms using the 
checkAvail ability() method. 
To access a property of this 
object, the object name is 
followed by a dot (the period 
symbol) and the name of the 
property that you want. 
Similarly, to use the method, 
you can use the object name 
followed by the method name. 
hotel . checkAvailability() 
If the method needs parameters, 
you can supply them in the 
parentheses (just like you can 
pass arguments to a function). 


2.  CREATING OBJECTS USING 
CONSTRUCTOR SYNTAX
 
ex : var hotel = new Object(); 

explain : 

an empty object  
called hotel is created using the 
constructor function. 
Once it has been created, three 
properties and a method are 
then assigned to the object. 
(If the object already had any 
of these properties, this would 
overwrite the values in those 
properties.) 
To access a property of this 
object, you can use dot notation, 
just as you can with any object. 
For example, to get the hotel's 
name you could use: 
hotel .name 
Similarly, to use the method, 
you can use the object name
followed by the method name: 
hotel.checkAvailability() 



3. CREATE & ACCESS OBJECTS 
CONSTRUCTOR NOTATION

**more explanation** : 
First, a constructor function 
defines a template for the hotels. 
Next, two different instances 
of this type of hotel object are 
created. The first represents 
a hotel called Quay and the 
second a hotel called Park. 
Having created instances of 
these objects, you can then 
access their properties and 
methods using the same dot 
notation that you use with all 
other objects. 
In this example, data from both 
objects is accessed and written 
into the page. (The HTML 
for this example changes to 
accommodate the extra hotel.) 
For each hotel, a variable is 
created to hold the hotel name, 
followed by space, and the word 
rooms. 
The line after it adds to that 
variable with the number of 
available rooms in that hotel. 
(The+= operator is used to add 
content to an existing variable.) 

4. ADDING AND REMOVING 
PROPERTIES 


If an object is created using a constructor function, this syntax only adds 
or removes the properties from the one instance of the object (not all 
objects created with that function). 


### THIS (IT IS A KEYWORD) 
The keyword this is commonly used inside functions and objects. 
Where the function is declared alters what this means. It always refers 
to one object, usually the object in which the function operates. 

### STORING DATA
In JavaScript, data is represented using name/value pairs. 
To organize your data, you can use an array or object to group a set of 
related values. In arrays and objects the name is also known as a key.

1. VARIABLES 
A variable has just one key (the variable name) 
and one value. 

2. ARRAYS 
Arrays can store multiple pieces of information. 
Each piece of information is separated by a comma. 
The order of the values is important because items 
in an array are assigned a number (called an index). 
Values in an array are put in square brackets, 
separated by commas: 


# Document Object Model
The Document Object Model (DOM) specifies 
how browsers should create a model of an HTML 
page and how JavaScript can access and update the 
contents of a web page while it is in the browser window


**THE DOM TREE IS A** 
MODEL OF A WEB PAGE 
As a browser loads a web page, it creates a model of that page. 
The model is called a DOM tree, and it is stored in the browsers' memory. 
It consists of four main types of nodes. 


### WORKING WITH THE DOM TREE 
Accessing and updating the DOM tree involves two steps: 
1: Locate the node that represents the element you want to work with. 
2: Use its text content, child elements, and attributes. 


STEP 1: ACCESS THE ELEMENTS
* SELECT AN INDIVIDUAL ELEMENT NODE
* SELECT MULTIPLE ELEMENTS (NODELISTS)
* TRAVERSING BETWEEN ELEMENT NODES 

STEP 2: WORK W ITH THOSE ELEMENTS
* ACCESS/ UPDATE TEXT NODES
* WORK W ITH HTML CONTENT
* ACCESS OR UPDATE ATTRIBUTE VALUES 

### ACCESSING ELEMENTS 
DOM queries may return one element, or they may return a Nodelist, 
which is a collection of nodes. 

**METHODS THAT RETURN A SINGLE ELEMENT NODE:** 
1. getElementByld( 1 id 1) 
Selects an individual element given the value of its i d attribute . 
The HTML must have an id attribute in order for it to be selectable. 
First supported: IE5.5, Opera 7, all versions of Chrome, Firefox, Safari. 
2. querySel ector( 1css selector') 
Uses CSS selector syntax that would select one or more elements . 
This method returns only the first of the matching elements. 
First supported: IE8, Firefox 3.5, Safari 4. Chrome 4, Opera 10 
... 
get ElementByld('one') 
... 
querySelector('l i . hot ' ) 
METHODS THAT RETURN ONE OR MORE ELEMENTS (AS A NODELIST): 
3. getEl ementsByClassName( 1class 1) 
Selects one or more elements given the value of their cl ass attribute. 
The HTML must have a cl ass attribute for it to be selectable. 
This method is faster than querySe 1ectorA11 () . 
First supported: IE9, Firefox 3, Safari 4, Chrome 4, Opera 10 
(Several browsers had partial I buggy support in earlier versions) 
4. getEl ementsByTagName( 1tagName 1) 
Selects all elements on the page with the specified tag name. 
This method is faster than querySe 1ectorA11 (). 
First supported: IE6+, Firefox 3, Safari 4, Chrome, Opera 10 
(Several browsers had partial I buggy support in earlier versions) 
5. querySelectorAll ( 1css select or•) 
Uses CSS selector syntax to select one or more elements and returns all 
of those that match. 


### LOOPING THROUGH A NODELIST 
If you want to apply the same 
code to numerous elements, 
looping through a Nodelist is a 
powerful technique.

JAVASCRIPT It involves finding out how many 
items are in the Nodelist, and 
then setting a counter to loop 
through them, one-by-one. 

Each time the loop runs, the 
script checks that the counter 
is less than the total number of 
items in the Nodelist. 

### TRAVERSING THE DOM 
When you have an element node, you can select 
another element in relation to it using these five 
properties. This is known as traversing the DOM

**ACCESS & UPDATE A TEXT NODE WITH NODEVALUE** 
When you select a text node, you can retrieve or amend the content of it 
using the node Va 1 ue property. 

**ACCESSING & CHANGI NG A TEXT NODE** 
To work with text in an element, 
first the element node is 
accessed and then its text node. 
JAVASCRIPT 
The text node has a property 
called node Value which returns 
the text in that text node
You can also use the node Va 1 ue 
property to update the content 
of a text node.

### ACCESS & UPDATE TEXT & MARKUP WITH INNERHTML 
Using the i nnerHTML property, you can access 
and amend the contents of an element, 
including any child elements. 

1. UPDATE TEXT & MARKUP 
2.ADDING ELEMENTS USING DOM MANIPULATION
* CREATE THE ELEMENT
* GIVE IT CONTENT
* ADD IT TO THE DOM

### ADDING AN ELEMENT TO THE DOM TREE 
createEl ement () creates an 
element that can be added to the 
DOM tree, in this case an empty 
`<l i>`~element for the list. 
JAVASCRIPT 
This new element is stored 
inside a variable called newEl 
until it is attached to the DOM 
tree later on.

### REMOVING ELEMENTS VIA DOM MANIPULATION 
DOM manipulation can be used to remove 
elements from the DOM tree

### XSS: VALIDATION & TEMPLATES 
Make sure that your users can only input characters they need to use 
and limit where this content will be shown on the page. 

### XSS: ESCAPING & CONTROLLING MARKUP 
Any content generated by users that contain characters that are used 
in code should be escaped on the server. You must control any markup 
added to the page. 

## CREATING ATTRIBUTES & CHANGING THEIR VALUES 
The cl assName property allows 
you to change the value of the 
cl ass attribute. If the attribute 
does not exist, it will be created 
and given the specified value
You have seen this property 
used throughout the chapter 
to update the status of the 
list items. Below, you can see 
another way to achieve the task. 
The setAttri bute() method 
allows you to update the value 
of any attribute. It takes two 
parameters: the attribute name, 
and the value for the attribute.

## REMOVING ATTRI BUTES 
To remove an attribute from an 
element, first select the element, 
then call removeAtt r i bute () . 
It has one parameter: the name 
of the attribute to remove. 
JAVASCRIPT 
Trying to remove an attribute 
that does not exist will not cause 
an error, but it is good practice 
to check for its existence before 
attempting to remove it. 
In this example, the 
get El ementByld () method is 
used to retrieve the first item 
from this list, which has an id 
attribute with a value of one.

## EXAMINING THE DOM IN FIREFOX 
Firefox has similar built-in tools, but you can 
also download a DOM inspector tool that 
shows the text nodes. 
