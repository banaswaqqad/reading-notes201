 # Lists 

there are three different types of lists : 
1. Ordered Lists created by `<ol>`
`<li>`
Each item in the list is placed 
between an opening `<li>` tag 
and a closing `</li>` tag. (The li
stands for list item.)

2. Unordered List created by `<ul>` tag 
`<li>`
Each item in the list is placed 
between an opening `<li>` tag 
and a closing `</li>` tag. (The li
stands for list item.)

3. Definition Lists created by `<dl>` tag 

inside the `<dl>` element you will 
usually see pairs of `<dt>` and 
`<dd>` elements.
`<dt>`
This is used to contain the term 
being defined (the definition 
term).
`<dd>`
This is used to contain the 
definition.

Nested list:  You can put a second list inside 
an `<li>` element to create a sub￾list or nested list

# Boxes

Controlling size of boxes

to set Box Diminsions use width, height 

there any many ways : 
1. pixels : the most popular method 
because they allow designers to 
accurately control their size
2. percentages :the size of the box based on the size of the containing box
3. ems : the size 
of the box is based on the size 
of text within it


**Limiting Width** 
* min-width, max-width : very helpful properties 
to ensure that the content of 
pages are legible (especially on 
the smaller screens of handheld 
devices
* min-height, max-height : to limit the height 


**Overflowing content**
when there is not 
enough space for the content of 
a box, you can use the overflow
property

It can have 
one of two values:

1. hidden
This property simply hides any 
extra content that does not fit in 
the box.

2. scroll
This property adds a scrollbar to 
the box so that users can scroll 
to see the missing content.

**border,margin and padding**

1. Border : The border 
separates the edge of one box 
from another.
2. You can set the 
width of a margin to create a 
gap between the borders of two 
adjacent boxes.
3. Padding is the space between 
the border of a box and any 
content contained within it. 

**BORDER**

* border-width : you can set border width 
border-top-width
border-right-width
border-bottom-width
border-left-width

* border-style 
1. solid: a single solid line
dotted a series of square dots
2. groove : be carved 
into the page
3. ridge: appears to stick out from 
the page
4. inset :  embedded into 
the page
5. outset : looks like it is coming 
out of the screen
6. hidden : none no border is 
shown

**PADDING**
padding-top
padding-right
padding-bottom
padding-left

**margin**
margin-top
margin-right
margin-bottom
margin-left


**display:** you can change elements from inline to block and from block to inline 

* inline : This causes a block-level 
element to act like an inline 
element.
* block : This causes an inline element to 
act like a block-level element.
* inline-block This causes a block-level 
element to flow like an inline 
element, while retaining other 
features of a block-level element.
* none : This hides an element from the 
page

**Hiding Boxes visibility**

**Quize** 

explain what do you know about Hiding Boxes visibility? 

**border-image**

The border-image property 
applies an image to the border of 
any box. It takes a background 
image and slices it into nine 
pieces

This property requires three 
pieces of information:
1. The URL of the image 
2. Where to slice the image
3. What to do with the straight 
edges; the possible values are:
 * **stretch** stretches the image
 * **repeat** repeats the image
 * **round** like repeat but if the 
tiles do not fit exactly, scales 
the tile image so they will

**box-shadow** : allows you to add a drop shadow around a box

It must 
use at least the first of these two 
values as well as a color:
Horizontal offset

Vertical offset

Blur distance

Spread of shadow

**Rounded Corners**
using a property called 
border-radius. The value 
indicates the size of the radius 
in pixels.

border-top-right-radius
border-bottom-right-radius
border-bottom-left-radius
border-top-left-radius


 

### WHAT IS A VARIABLE? 
a space you can store (int,strings,bool) and it might be changed 

**you can declare variable by**
example : 
`var age = 50;` >>> store numbers 
` var username = 'bana' ` >>> store strings 
` var isexist = true ` >>> store boolean

### DATA TYPES 

we have three main data types 

1. numbers : (1-9)
2. strings : (every char in keyboard)
3. bool : (`true and false`)

**the variable value might be changed** 

### ARRAYS 
An array is a special type of variable. It doesn't 
just store one value; it stores a list of values.

**Arrays are especially helpful when you do not know how many items a list will contain**

#### CREATING AN ARRAY 

example : 

`var colors;` 
`colors ['white', 'black', ' custom'];` 
`var el document.getElementByld('col ors');` 
`el . textContent = col ors[O];` 

### EXPRESSIONS : two types 
1. EXPRESSIONS THAT JUST ASSIGN A 
VALUE TO A VARIABLE 
example :` var color = 'beige';` 

2. EXPRESSIONS THAT USE TWO OR 
MORE VALUES TO RETURN A 
SINGLE VALUE 
example : `var area = 3 * 2;`

### OPERATORS

1. ASSIGNMENT OPERATORS : Assign a value to a variable
2. COMPARISON OPERATORS : Compare two values and return true or fa 1 se
3. ARITHMETIC OPERATORS : Perform basic math  
4. LOGICAL OPERATORS : Combine expressions and return true or fa 1 se
5. STRING OPERATORS : Combine two strings 


### Decisions and Loops

**loops**
1. FOR LOOPS
The loop starts with the for 
keyword, then contains the 
condition inside the parentheses. 
As long as the counter is less 
than the total number of items 
in the array, the contents of the 
curly braces will continue to 
run. Each time the loop runs, the 
round number is increased by 1.

2. WHILE LOOPS : 
This loop will continue to run 
for as long as the condition in 
the parentheses is true

3. DO WHILE LOOPS : 
The key difference between 
a while loop and a do while 
loop is that the statements in 
the code block come before the 
condition. This means that those 
statements are run once whether 
or not the condition is met
