#**HTML "Structure"** 

1. what do mean with "HTML Uses Elementsto Describe the Structure of Pages ? "
in html we have parents tags 


Tags act like containers. They tell you 
something about the information that lies 
between their opening and closing tags


<html> >>> opening tag
</html> >>> closing tag 

The opening <html> tag indicates that anything between it and a closing </html> tag is HTML code. 
**this is how we start our html page** 
then we have the body tag 

<body> </body>

The <body> tag indicates that anything between it and the closing 
</body> tag should be shown inside the main browser window.

in the body we can use too many tags like 

1. <h1> and </h1>  Words between those tags are a main heading.
2.  <h2> and </h2> Words between form a sub-heading.
3. <p> and </p> A paragraph of text appears between these

notes : 1. to open the tag we use these signs < >
        2. to close the tag we put / after the less-than sign </>


**now we will talk about Attributes to explain More About Elements**

Attributes provide additional information 
about the contents of an element. They appear 
on the opening tag of the element and are 
made up of two parts: a name and a value, 
separated by an equals sign.

<p lang="en-us">Paragraph in English</p>
p : is element 
lang : is attribute name 
en-us : attribute value 



now your turn ,  Try to separate out this example 

<h1 "color = blue" > hello people </h1>



#**“Extra Markup**

**different versions of HTML and how to indicate which version you are using**

1. what is doctypes and what is the aim to use it ? 

each web page should begin with a 
DOCTYPE declaration to tell a 
browser which version of HTML 
the page is using (although 
browsers usually display the 
page even if it is not included). 

2. Comments in html :
if you want add notes to help you and other programmer in understanding your code you can add somthing called **comments**
 
adding comment to your code  will not be 
visible in the user's browser, you 
can add the text between these 
characters:
<!-- comment goes here -->


3. ID Attribute : 
Every HTML element can carry 
the id attribute. It is used to 
uniquely identify that element 
from other elements on the 
page. Its value should start with 
a letter or an underscore (not a 
number or any other character).
It is important that no two 
elements on the same page 
have the same value for their id
attributes (otherwise the value is 
no longer unique).


4. Class Attribute : 

we use this attributes if we want to style multiple elemnts at the same time just we put the name of class in the opening tag 
example : <p class="answer">

5. Inline Elements 

Some elements will always 
appear to continue on the 
same line as their neighbouring 
elements. These are known as 
inline elements.
example : <a>, <b>, <em>, and <img>.


6. Grouping Text & 
Elements In a Block


* <div> : 

The <div> element allows you to 
group a set of elements together 
in one block-level box

For example, you might create 
a <div> element to contain all 
of the elements for the header 
of your site (the logo and the 
navigation), or you might create 
a <div> element to contain 
comments from visitors.

* <span> 

The most common reason why 
people use <span> elements 
is so that they can control the 
appearance of the content of 
these elements using CSS 


**the <span>**
1. Contain a section of text 
where there is no other suitable 
element to differentiate it from 
its surrounding text
2. Contain a number of inline 
elements

* <iframe> 

An iframe is like a little window 
that has been cut into your 
page — and in that window you 
can see another page. The term 
iframe is an abbreviation of inline 
frame.

An iframe is created using the  
<iframe> element. There are a 
few attributes that you will need 
to know to use it:

1. src
The src attribute specifies the 
URL of the page to show in the 
frame.
2. height
The height attribute specifies 
the height of the iframe in pixels.
3. width
The width attribute specifies 
the width of the iframe in pixels.


**extra Information About Your Pages**

<meta>
The <meta> element lives 
inside the <head> element and 
contains information about that 
web page.
It is not visible to users but 
fulfills a number of purposes 
such as telling search engines 
about your page, who created 
it, and whether or not it is time 
sensitive. (If the page is time 
sensitive, it can be set to expire.)
The <meta> element is an empty 
element so it does not have a 
closing tag. It uses attributes to 
carry the information.


**Escape CharaCtErs**
There are some characters that are used in 
and reserved by HTML code. (For example, the 
left and right angled brackets.)

!(escape characters)[https://slideplayer.com/slide/14037584/86/images/16/Text+Appearance+HTML+code+Meaning+Escape+Character+%26+%26amp+Ampersand.jpg]


**#HTML5 Layout**

1. Headers & Footers

these elements are appear at the top or 
bottom of every page on the 
site. 

**i can help and tell that you can put copy write sign in footer**

2. Navigation <nav>

The <nav> element is used to 
contain the major navigational 
blocks on the site such as the 
primary site navigation.

3. Articles <article> 

The <article> element acts as 
a container for any section of a 
page that could stand alone and 
potentially be syndicated.
This could be an individual 
article or blog entry, a comment 
or forum post, or any other 
independent piece of content.
If a page contains several articles 
(or even summaries of several 
articles), then each individual 
article would live inside its own 
<article> element.
The <article> elements can 
even be nested inside each 
other

4. Asides <aside>

The <aside> element has two 
purposes, depending on whether 
it is inside an <article>
element or not.

1. When the <aside> element 
is used inside an <article>
element, it should contain 
information that is related to the 
article but not essential to its 
overall meaning.

2. When the <aside> element is 
used outside of an <article>
element, it acts as a container 
for content that is related to 
the entire page

5. Sections
<section>

The <section> element groups 
related content together, and 
typically each section would 
have its own heading.

because the <section> element 
groups related items together, 
it may contain several distinct 
<article> elements that have a 
common theme or purpose. 
Alternatively, if you have a 
page with a long article, the 
<section> element can be 
used to split the article up into 
separate sections.
The <section> element should 
not be used as a wrapper for 
the entire page (unless the 
page only contains one distinct 
piece of content). If you want a 
containing element for the entire 
page, that job is still best left to 
the <div> element.

6. Heading Groups
<hgroup>

The purpose of the <hgroup>
element is to group together a 
set of one or more <h1> through 
<h6> elements so that they are 
treated as one single heading. 

7. Figures
<figure> <figcaption>

Examples of usage of figures include:
● Images
● Videos
● Graphs
● Diagrams
● Code samples
● Text that supports the main 
body of an article
The <figure> element should 
also contain a <figcaption>
element which provides a text 
decription for the content of 
the <figure> element. In 
this example, you can see a 
<figure> has been added inside 
the <article> element.


**#Process & Design**

before bulding any sites you should ask yourself  the **four W questions**

1. why 
2. what 
3. how 
4. who
 

 **Who is the Site For?**

you can  Target Audience: individuals by ask some questions like :

*  What is the age range of your target audience?
*  Will your site appeal to more women or men? What is the mix?
*  Which country do your visitors live in?
*  Do they live in urban or rural areas?
*  What is the average income of visitors?
*  What level of education do they have?
*  What is their marital or family status?
*  What is their occupation?
*  How many hours do they work per week?
*  How often do they use the web?
*  What kind of device do they use to access the web?


also you can  Target Audience: Companies by ask some questions like :

* What is the size of the company or relevant department?
* What is the position of people in the company who visit your site?
* Will visitors be using the site for themselves or for someone else?
* How large is the budget they control?


**Why People Visit YOUR Website**
Now after you know who your visitors are, you 
need to consider why they are coming. 

this question has 2 basic things should know them 

1.  motivations for 
why visitors come to the site.
2.  goals of the visitors. 

**Motivations**
* Are they looking for general 
entertainment or do they 
need to achieve a specific 
goal? 
* If there is a specific goal, is 
it a personal or professional 
one?
* Do they see spending time on 
this activity as essential or a 
luxury?

**Goals**

* Do they want general 
information / research (such 
as background on a topic / 
company), or are they after 
something specific (such as a 
particular fact or information 
on a product)?

* Are they looking for time 
sensitive information, such as 
the latest news or updates on 
a particular topic?
* Do they want to discover 
information about a specific 
product or service to help 
them decide whether to buy 
it or not?

* Do they need to contact you? 
If so, can they visit in person 
(which might require opening 
hours and a map)? Or might 
they need email or telephone 
contact details?

**What Information Your Visitors Need**

You know who is coming to your site and why 
they are coming, so now you need to work out 
what information they need in order to achieve 
their goals quickly and effectively.

these questions will help you 

* Will visitors be familiar with 
your subject area / brand 
or do you need to introduce 
yourself?
* Will they be familiar with 
the product / service / 
information you are covering 
or do they need background 
information on it?
* What are the most important 
features of what you are 
offering?
* What is special about what 
you offer that differentiates 
you from other sites that offer 
something similar?
* Once people have achieved 
the goal that sent them to 
your site, are there common 
questions people ask about 
this subject area?


**How Often People Will Visit Your Site**

Some sites benefit from being updated more 
frequently than others. Some information (such 
as news) may be constantly changing, while 
other content remains relatively static.

Once a site has been built, it can 
take a lot of time and resources 
to update it frequently.
Working out how often people 
are likely to revisit your site gives 
you an indication for how often 
you should update the site.
It can often be helpful to set a 
schedule for when a site will be 
updated (rather than doing it on 
an ad hoc basis).
You will often find that some 
parts of a site will benefit from 
being updated more frequently 
than others.

**Here are some questions to help you decide how often to update your website content...**

* How often do the same 
people return to purchase 
from you?
* How often is your stock 
updated or your service 
changed?
Information
* How often is the subject 
updated?
* What percentage of your 
visitors would return for 
regular updates on the 
subject, compared with 
those who will just need the 
information once?

**Site Maps**

The aim is to create a diagram 
of the pages that will be used 
to structure the site. This is 
known as a site map and it will 
show how those pages can be 
grouped.


To help you decide what 
information should go on each 
page, you can use a technique 
called **card sorting.**

This involves placing each 
piece of information that a 
visitor might need to know on 
a separate piece of paper and 
then organizing the related 
information into groups.
Each group relates to a page and, 
on larger sites the, pages can in 
turn can be grouped together to 
create different sections of the 
website.
The groups of information are 
then turned into the diagram 
that is known as the site map.
Sometimes it can be helpful to 
ask people who are the target 
audience to help you group 
related information together.

!(card sorting example)[https://www.webfx.com/blog/images/assets/cdn.sixrevisions.com/0108-04_open_card_sorting2.png]


**WireFrames**
A wireframe is a simple sketch of the key 
information that needs to go on each page of a 
site. It shows the hierarchy of the information 
and how much space it might require.

