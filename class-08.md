# Layout :  
### Controlling the Position of Elements :

1. Normal flow : Every block-level element appears on a new line 
2. Relative Positioning :
 This moves an element from the 
position it would be in normal 
flow, shifting it to the top, right, 
bottom, or left of where it 
would have been placed.
3. Absolute positioning
positions the element 
in relation to its containing 
element. (It is taken out of 
normal flow)

**To indicate where a box should be positioned, you may also need to use box offset properties**

### NORMAL FLOW : 
position:static 

### Relative Positioning : 
position:relative 

### Absloute Positioning
position:absolute

### Fixed Positioning : 
position:fixed

## Floating ELEMENTS : 
**float** : 

The float property allows you 
to take an element in normal 
flow and place it as far to the 
left or right of the containing 
element as possible.
Anything else that sits inside 
the containing element will 
flow around the element that is 
floated.
When you use the float
property, you should also use the 
*width property* to indicate how 
wide the floated element should 
be.

####  USING FLOATS TO PLACE Elements Side-by-Side

`body {`
`width: 750px;`
`font-family: Arial, Verdana, sans-serif;`
`color: #665544;}`
`p {`
`width: 230px;`
`float: left;`
`margin: 5px;`
`padding: 5px;`
`background-color: #efefef;}`


## Screen Sizes : 
The size of a user's screen 
affects how big they can open 
their windows and how much 
of the page they will see. There 
are also an increasing number 
of handheld devices (mobile 
phones and tablets) that have 
smaller screens.

## Screen Resolution
**Resolution refers to the number of dots a screen shows per inch**

## Page Sizes : 

1. ### Fixed Width Layouts: 

**Advantages**
*  controlling size and 
positioning of elements.
* The designer has far greater 
control over the appearance 
and position of items on the 
page than with liquid layouts.
* You can control the lengths 
of lines of text regardless of 
the size of the user's window.
* The size of an image will 
always remain the same 
relative to the rest of the 
page.

**Disadvantages**
* You can end up with big gaps 
around the edge of a page.
* If the user's screen is a much 
higher resolution than the 
designer's screen, the page 
can look smaller and text can 
be harder to read.
* If a user increases font sizes, 
text might not fit into the 
allotted spaces.


 2. ### Liquid Layouts : 
**Advantages**
* Pages expand to fill the entire 
browser window so there are 
no spaces around the page 

* if the user have small window there is no need to scroll down  

**Disadvantages**
* if the user has a wide 
window, lines of text can 
become very long, which 
makes them harder to read.
* If the user has a very narrow 
window, words may be 
squashed and you can end up 
with few words on each line


# MULTIPLE STYLE SHEETS 

There are two ways to add 
multiple style sheets to a page:
1. Your HTML page can link 
to one style sheet and that 
stylesheet can use the @import
rule to import other style sheets.

2. In the HTML you can use a 
separate <link> element for 
each style sheet.
