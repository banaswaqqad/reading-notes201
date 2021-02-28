# Text 

**Headings and paragraphs**

When creating a web page, you add tags (known as markup) to the contents of the page 

**what is the aim from the these tags ?**

tags provide extra meaning and allow browsers to show users the appropriate structure for the page

there are two types of markup : 

1. Structural markup: the elements that you can use to 
describe both headings and paragraphs

2. Semantic markup: which provides extra information; such 
as where emphasis is placed in a sentence, that something 
you have written is a quotation (and who said it), the 
meaning of acronyms, and so on


# Headings

what is the different between  `/<h1> ... <h6>/`  levels ?

  `<h1>` >>>> indicate the importance of section 


# PARAGRAPHS 

to create a paragraph open `<p>`
tag and close it `</p>` .

# Bold & Italic 

* By enclosing words in the tags 
`<b> and </b>` we can make 
characters appear bold


* By enclosing words in the tags 
`<i> and </i>` we can make 
characters appear italic.

# Superscript &  Subscript 

**what is the different between Superscript & Subscript ?**


The `<sup>` element is used 
to contain characters that 
should be superscript such 
as the suffixes of dates or 
mathematical concepts like 
raising a number to a power such 
as 22
.

The `<sub>` element is used to 
contain characters that should 
be subscript. It is commonly 
used with foot notes or chemical 
formulas such as H2
0.


# White Space 

**what is white space collapsing?**

count two spaces as one space to make reading code easier


# Line Breaks & Horizontal Rules
* `<br/>`
 start new line 
* `<hr />`
To create a break between 
themes act like a "____"

# Strong & Emphasis 

 `<strong>`
The use of the `<strong>` 

**content has strong importance**

`<em>`
The `<em>` >>>>  subtly changes the meaning of a sentence

# Quotations 

1. `<blockquote>`
this element is 
used for longer quotes that take 
up an entire paragraph 
2. `<q>`
This  element is used for 
shorter quotes that sit within 
a paragraph

# Abbreviations & Acronyms

`<abbr>` >> A titleattribute on the opening tag is used to specify the full term **it's used for both abbreviations and acronyms.**

# Citations & Definitions : 

* `<cite>` element can be used to indicate where the citation is from.
* `<dfn>`  element is used to indicate the defining instance of a new term.

 # Author Details : 

 `<address>`

contain contact details for the author of the page.

# Changes to CONTENT

1. `<ins>`  show content that has been inserted into a document

2. `<del>` show text that has been deleted from it.

3. `<s>`  somthing should not be deleted 



# Understanding CSS : CASCADING STYLE SHEET (HOW THE PAGE SHOULD LOOK)

**in this part you should know about selectors and declaration**

we have 3 types of selectors in css we will mention it in this page but first you should know how the selector look and the declaration 
 
`P {   }` >>> in this example p is the selector and between the curly brackets is the declaration 

 Selectors indicate which element the rule applies to.

 Declarations indicate how the elements referred to in the selector should be styled 

 **you can in one statment use more than one selectors : 
 example : 

 `h1, h2, h3 {`
`font-family: Arial;`
 `color: yellow;}`


# Using External CSS : best one 

you should create separet file (style.css) and link it with the html page using `<link>`  tag : 

 `<link>` 
this element  used 
in an HTMLpage  to tell the 
browser where to find the CSS 
file  to style the page. It is an 
empty element (meaning it does 
not need a closing tag), you should write it
 inside the `<head>` element. 
It should use three attributes:

1. href
This specifies the path to the 
CSS file 
2. type
This attribute specifies the type 
of document being linked to. The 
value should be text/css.
3. rel
This specifies the relationship 
between the HTML page and 
the file it is linked to. 

**When building a site with more than one page, you should use an external CSS style shee**


# Using Internal css : not preferd 

use `<style>`  *placed in the head tag after the meta tag* and close it `<style/>`



when we style using Internal css , we should use css selectors .

**CSS Selectors**

There are many different types 
of CSS selectors . 

1. Universal Selector  >>> `* {}` Targets all elements on the page
2. Type Selector >>>  `h1, h2, h3 {}`  Targets the `<h1>`, `<h2>` and `<h3>` elements
3. Class Selector >>>`.note {} `  Targets any element whose classattribute has a value of note `p.note {}` Targets only `<p>` elements whose class attribute has a value of note

4. ID Selector >>> `#introduction {} ` Targets the element whose id attribute has a value of introduction
5. Child Selector >>> ` li>a {}` Targets any `<a>` elements that are children of an `<li>` element (but not other `<a>` elements in the page) 
6. Descendant Selector >>> `p a {} `  Targets any `<a>` elements that sit inside a `<p>` element, even if there are other elements nested between them
 
7. Adjacent Sibling Selector >>> 
8. General Sibling Selector >>> 

**i will let the 7 , 8 selectores for you to find the using of them**

# INHERETANCE : 

It saves you from having to apply 
 properties to as many 
elements (and results in simpler 
style sheets)


# WHAT IS A VARIABLE? 
a space you can store (int,strings,bool) and it might be changed 

**you can declare variable by**
example : 
`var age = 50;` >>> store numbers 
` var username = 'bana' ` >>> store strings 
` var isexist = true ` >>> store boolean

# DATA TYPES 

we have three main data types 

1. numbers : (1-9)
2. strings : (every char in keyboard)
3. bool : (`true and false`)

**the variable value might be changed** 

# ARRAYS 
An array is a special type of variable. It doesn't 
just store one value; it stores a list of values.

**Arrays are especially helpful when you do not know how many items a list will contain**

# CREATING AN ARRAY 

example : 

`var colors;` 
`colors ['white', 'black', ' custom'];` 
`var el document.getElementByld('col ors');` 
`el . textContent = col ors[O];` 


# VALU ES IN ARRAYS 


Values in an array are accessed as if they are in 
a numbered list. It is important to know that the 
numbering of this list starts at zero (not one). 
NUMBERING ITEMS IN 
AN ARRAY 
Each item in an array is 
automatically given a number 
called an index. This can be used 
to access specific items in the 
array



