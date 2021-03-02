# Links 

1. Writing Links : Links are created using the `<a>` element
2. The text between the opening 
`<a>` tag and closing `</a>` tag 
is known as link text.

(To write good link text, you can 
think of words people might 
use when searching for the 
page that you are linking to)

3. Linking to Other Sites 

* href: The value of the 
href attribute is the page that 
you want people to go to when 
they click on the link

* Absolute URLs : This is the 
web address that you would type 
into a browser if you wanted to 
visit that specific page.

4. Linking to Other Pages on the Same Site : You can use a shorthand known as a 
`**relative URL.**`

`### Relative URLs :` 
help when building  a site on your computer because 
you can create links between 
pages without having to set up 
your domain name or hosting.


## Directory Structure :
 1. Structure : placing the pages for each different section of the site into a new folder.
 2. Relationships : The relationship between files and folders on a website
 3. Homepages : The main homepage of a site written in HTML (called index.html.)

 # Relative URLs : 

 ### Relative URLs can be used when linking to pages within your own website. 
    **They provide a shorthand way of telling the browser where to find your files**
    **you do not need to repeat the domain name in each link, they are also quicker to write**

## Relative Link Types : 
1. Same Folder :
 To link to a file in the same folder, just use the file name
2. Child Folder :
 use the name of the child folder, followed by a forward slash, then the file name.
3. Grandchild FolderUse the name of the child folder, followed by a forward slash, then the name of the grandchild folder, followed by another forward slash, then the file name.
4. Parent Folder :
Use ../ to indicate the folder above the current one, 
then follow it with the file name
5. GrandParent Folder : 
Repeat the ../ to indicate that you want to go up 
two folders (rather than one), then follow it with the 
file name.

### Email Links : 

use the `<a>`
element and the value of the href attribute starts 
with mailto: and is followed by 
the email address you want the 
email to be sent to.

### Opening Links in a New Window : 
If you want a link to open in a 
new window, you can use the 
target attribute on the opening 
`<a>` tag. The value of this 
attribute should be _blank.


### Linking to a Specific Part of the Same Page : 
by :
 1. identify the points in the page 
that the link will go to. You do 
this using the id attribute
 2. the value of the href in `<a>` starts with 
 the # symbol, followed by the 
 value of the id attribute of the 
 element you want to link to

 ### Linking to a Specific Part of Another Page

 by :
 1. identify the points in the page 
that the link will go to. You do 
this using the id attribute
 2. the value of the href in `<a>` starts with 
 the # symbol, followed by the 
 value of the id attribute of the 
 element you want to link to and the href attribute 
will contain the address for the 
page 

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


# WHAT IS A FUNCTION? 
group a series of statements together to perform a 
specific task it's reuasable 

## Declaring function 
function word then name of the function then ()  then the statment you should be in the function  
example : 

`function updateMessage() {` 
`var el = document.getElementByld('message'};` 
`el .textContent = msg;` 
`}

## calling function :

 `function updateMessage(parametirs) { `
`var el = document.getElementByld('message'};` 
`el .textContent = msg;` 
`}` 
`updateMessage(};` 

## Declaring function That need info 
function word then name of the function then ( inside it you send parametires )  then the statment you should be in the function  
example : 

## calling function That need info 
function word then name of the function then ()  then the statment you should be in the function  
example : 

` function updateMessage(parametirs) {` 
`var el = document.getElementByld('message'};` 
`el .textContent = msg; `
`} `
`updateMessage(the thing you would send it )};` 


# 6 Reasons for Pair Programming 

1. ### How does pair programming work? 

pair programming commonly involves two roles: 
1.  **Driver** : The Driver is the programmer who is typing and the only one whose hands are on the keyboard , the Driver manages the text editor, switching files, version control, and—of course writing—code
2. **Navigator** : 
* uses their words to guide the Driver but does not provide any direct input to the computer
* thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs.
* utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code

2. ### Why pair program? 

**there are four fundamental skills that help anyone learn a new language: Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea Reading: understanding what written language intends to convey Writing: producing from scratch a meaningful**

### **Pair programming touches on all four skills**:
 1. developers explain out loud what the code should do
 2. listen to others’ guidance
 3. read code that others have written
 4. and write code themselves.

 ### 1. Greater efficiency : 
 **how ?**
 when coming up with ideas and discussing solutions out loud, two programmers may come to a solution faster than one programmer on their own. Also, when the pair is stuck, both programmers can research the problem and reach a solution faster. Researches also identified pairing enhances technical skills, team communication, and even enjoyability of coding in the workplace 

###  2. Engaged collaboration : 
When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone
Another important aspect of learning to program is knowing when to ask for help.

### 3. Learning from fellow students 

## 4.Social skills 
 Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key.

### 5. Job interview readiness : 

They will carry out exercises together, such as code challenges, building a project or feature, or debugging an existing code base. By doing so, companies can get a better feel for how an applicant will fit into the team and their collaboration style.

### 6.  Work environment readiness : 

Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.