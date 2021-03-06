# Images

### Adding Images steps : 
1. To add an image into the page 
you need to use an `<img>`
element
2. use `src` : This tells the browser where 
it can find the image file
3. use `alt` : This provides a text description 
of the image which describes the 
image if you cannot see it.
4. title : You can also use the title
attribute with the `<img>` element 
to provide additional information 
about the image

### Height & Width of Images
* **height**
This specifies the height of the 
image in pixels.
* **width**
This specifies the width of the 
image in pixels.

## Where to Place Images in Your Code ? 
you can place your img any place you want (  before a paragraph,inside the start of a 
paragraph , in the middle of a paragraph ....etc  )

## Aligning Images : 
**used to indicate how the other parts of a page should flow around an image** 

1. Horizontally : 

* left
This aligns the image to the left 
(allowing text to flow around its 
right-hand side).
* right
This aligns the image to the right 
(allowing text to flow around its 
left-hand side).

2. Vertically : 
* top :
This aligns the first line of the 
surrounding text with the top of 
the image.
* middle :
This aligns the first line of the 
surrounding text with the middle 
of the image.
* bottom : 
This aligns the first line of the 
surrounding text with the bottom 
of the image.

### Three Rules for Creating Images
1. **Save images in  the right format** : 

types for images format : 
JPg and GIF
2. **Save images at the right size**

The images you use on your website should be 
saved at the same width and height that you 
want them to appear on the page.

3. Use the correct resolution 

The  resolution of an image is the 
number of squares that fit within 
a 1 inch x 1 inch square area.

Images created for the web should be saved at 
a resolution of 72 ppi. The higher the resolution 
of the image, the larger the size of the file.

JPGs, GIFs, and PNGs belong to 
a type of image format known 
as bitmap

**Vector Images** 

Vector images differ from bitmap images and 
are resolution-independent. Vector images are 
commonly created in programs such as Adobe 
Illustrator.

**Animated GIFs** 

Animated GIFs show several frames of an 
image in sequence and therefore can be used to 
create simple animations

**Transparency** 

Creating an image that is partially transparent 
(or "see-through") for the web involves 
selecting one of two formats:
Transparent GIF and png 

# Color :
**The color property allows you to specify the color of text inside an element**.
 You can specify any color in CSS in one of three ways:
1. rgb values
These express colors in terms 
of how much red, green and 
blue are used to make it up. For 
example: rgb(100,100,90) 

RGB: **Values for red, green, and blue are expressed as numbers between 0 and 255**.


 2. hex codes
These are six-digit codes that 
represent the amount of red, 
green and blue in a color, 
preceded by a pound or hash # 
sign. For example: #ee3e80

Hex values: **represent values for red, green, and blue in hexadecimal code**

3. color names
There are 147 predefined color 
names that are recognized 
by browsers. For example: 
DarkCyan

Colors are **represented by predefined names. However, they are very limited in number**


### `background-color` 

The background-color property 
sets the color of the background 
for that box.
You can specify your choice of 
background color in the same 
three ways you can specify 
foreground colors: RGB values, 
hex codes, and color names 

### Contrast
1. Low Contrast
2. High Contrast
3. Medium Contrast

It is important to ensure that there is enough contrast 
between any text and the background color (otherwise 
people will not be able to read your content)

### Opacity 
CSS3 has introduced an extra value for RGB colors to 
indicate opacity. It is known as RGBA.

### HSL & HSLA 

CSS3 also allows you to specify colors as HSL values, 
with an optional opacity value. It is known as HSLA.
**HSL & HSLA  represent to**
* h stand for hue
This is expressed as an angle 
(between 0 and 360 degrees).
* s stand for saturation
This is expressed as a 
percentage.

* l stand for lightness
This is expressed as a 
percentage with 0% being white, 
50% being normal, and 100% 
being black.


### The hsla color : 
 property allows  you to specify color properties 
using hue, saturation, and 
lightness as above, and adds a 
fourth value which represents 
transparency (just like the rgba
property) but the: 

* a stand for alpha
This is expressed as a 
number between 0 and 1.0. 
For example, 0.5 represents 
50% transparency, and 0.75
represents 75% transparency.

# Text 

## Typeface Terminology 

1. Serif 
Serif fonts have extra details on 
the ends of the main strokes of 
the letters. These details are 
known as serifs

2. Sans-Serif
Sans-serif fonts have straight 
ends to letters, and therefore 
have a much cleaner design

3. Monospace
Every letter in a monospace (or 
fixed-width) font is the same 
width. (Non-monospace fonts 
have different widths) 

4. Weight :
The font weight not only adds 
emphasis but can also affect 
the amount of white space and 
contrast on a page.

5. Style : 
Italic fonts have a cursive aspect 
to some of the lettering. Oblique 
font styles take the normal style 
and put it on an angle.

6. Stretch  
In condensed (or narrow) 
versions of the font, letters are 
thinner and closer together. 
In expanded versions they are 
thicker and further apart. 

## Specifying Typefaces
1. font-family 

The font-family property 
allows you to specify the 
typeface that should be used for 
any text inside the element(s) to 
which a CSS rule applies.
The value of this property is the 
name of the typeface you want 
to use. 

2. Size of type :

`font-size`
The font-size property enables 
you to specify a size for the 
font. **There are several ways** to 
specify the size of a font. The 
most common are:

* pixels
Pixels are commonly used 
because they allow web 
designers very precise control 
over how much space their text 
takes up. The number of pixels is 
followed by the letters px.

* percentages
The default size of text in 
browsers is 16px. So a size of 
75% would be the equivalent of 
12px, and 200% would be 32px.

* ems
An em is equivalent to the width 
of a letter m.

### Understanding Font Format

1. Bold
**font-weight** : 
The font-weight property 
allows you to create bold text. 
There are two values that this 
property commonly takes:

* normal
This causes text to appear at a 
normal weight.
* bold
This causes text to appear bold.

2. ITALIC :
**font-style**
If you want to create italic text, 
you can use the font-style
property. There are three values 
this property can take:
* normal
This causes text to appear in a 
normal style (as opposed to italic 
or oblique).
* italic
This causes text to appear italic.
* oblique
This causes text to appear 
oblique.

3. UpperCase & LowerCase
**text-transform**
The text-transform property 
is used to change the case of 
text giving it one of the following 
values:
* uppercase
This causes the text to appear 
uppercase.
* lowercase
This causes the text to appear 
lowercase.
* capitalize
This causes the first letter of 
each word to appear capitalized

4. Underline & Strike
**text-decoration**
The text-decoration property 
allows you to specify the 
following values:
* none
This removes any decoration 
already applied to the text.
* underline
This adds a line underneath the 
text.
* overline
This adds a line over the top of 
the text.
* line-through
This adds a line through words.
* blink
This animates the text to make it 
flash on and off (however this is 
generally frowned upon, as it is 
considered rather annoying).

5. Leading
**line-height** 
Leading (pronounced ledding) is 
a term typographers use for the 
vertical space between lines of 
text. In a typeface, the part of 
a letter that drops beneath the 
baseline is called a descender, 
while the highest point of a letter 
is called the ascender. Leading 
is measured from the bottom of 
the descender on one line to the 
top of the ascender on the next.

6. Letter & Word Spacing
**letter-spacing, word-spacing**
Kerning is the term 
typographers use for the space 
between each letter. You can 
control the space between each 
letter with the letter-spacing
property.

7. Alignment
**text-align**
The text-align property allows 
you to control the alignment of 
text. The property can take one 
of four values:
* left
This indicates that the text 
should be left-aligned.
* right
This indicates that the text 
should be right-aligned.
* center
This allows you to center text.
* justify
This indicates that every line in 
a paragraph, except the last line, 
should be set to take up the full 
width of the containing box

8. Vertical Alignment
**vertical-align**

The vertical-align property is 
a common source of confusion. 
It is not intended to allow you to 
vertically align text in the middle 
of block level elements such as 
`<p>` and `<div>`, although it does 
have this effect when used with 
table cells (the `<td>` and `<th>`
elements).
It is more commonly used with 
inline elements such as `<img>`, 
`<em>`, or `<strong>` elements. 
When used with these elements, 
it performs a task very similar to 
the HTML align attribute used 
on the `<img>` element, which 
you met on pages 103-106. The 
values it can take are:
1. baseline
2. sub
3. super
4. top
5. text-top
6. middle
7. bottom
8. text-bottom

It can also take a length (usually 
specified in pixels or ems) or a 
percentage of the line height.

9. Indenting Text
**text-indent**
The text-indent property 
allows you to indent the first 
line of text within an element. 
The amount you want the line 
indented by can be specified in 
a number of ways but is usually 
given in pixels or ems.
It can take a negative value, 
which means it can be used 
to push text off the browser 
window.

## CSS3 : 
1. Drop Shadow
**text-shadow**

text shadow used to create a drop 
shadow, which is a dark version 
of the word just behind it and 
slightly offset.
 It can also be used 
to create an embossed effect by 
adding a shadow that is slightly 
lighter than the text.
The value of this property is 
quite complicated because it can 
take **three lengths** and a color for 
the drop shadow. 
* The first length:  indicates how 
far to the left or right the shadow 
should fall.
* The second value indicates the 
distance to the top or bottom 
that the shadow should fall.
* The third value is optional and 
specifies the amount of blur that 
should be applied to the drop 
shadow.
* The fourth value is the color of 
the drop shadow



2. First Letter or Line
**:first-letter, :first-line**
You can specify different values 
for the first letter or first line of 
text inside an element using
:first-letter and 
:first-line. 
Technically these are not 
properties. They are known as 
pseudo-elements.

3. Styling Links
**:link, :visited**

Browsers tend to show links 
in blue with an underline by 
default, and they will change 
the color of links that have been 
visited to help users know which 
pages they have been to.

In CSS, there are two pseudo￾classes that allow you to set 
different styles for links that 
have and have not yet been 
visited
:
* :link
This allows you to set styles 
for links that have not yet been 
visited. 
* :visited
This allows you to set styles for 
links that have been clicked on

4. Responding to Users
**:hover, :active, :focus**
There are three pseudo-classes 
that allow you to change the 
appearance of elements when a 
user is interacting with them.
* :hover : 
This is applied when a user 
hovers over an element with a 
pointing device such as a mouse. 
This has commonly been used 
to change the appearance of 
links and buttons when a user 
places their cursor over them. It 
is worth noting that such events 
do not work on devices that use 
touch screens (such as the iPad) 
because the screen is not able to 
tell when someone is hovering 
their finger over an element.
* :active :
This is applied when an element 
is being activated by a user; for 
example, when a button is being 
pressed or a link being clicked. 
Sometimes this is used to make 
a button or link feel more like it 
is being pressed by changing the 
style or position of the element 
slightly.
* :focus:
This is applied when an element 
has focus. Any element that 
you can interact with, such as a 
link you can click on or any form 
control can have focus.
Responding to Users
:hover, :active, :focus
Focus occurs when a browser 
discovers that you are ready to 
interact with an element on the 
page