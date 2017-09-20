# bootsrap-learning

Responsive Web Design
=====================

Responsive web design makes your web page look good on all devices.
Responsive web design uses only HTML and CSS.
Resize, hide, shrink, enlarge, or move the content to make it look good on any screen.

viewport 
========

User's visible area of a webpage
varies with device

setting a view port 
<pre>
meta name="viewport" content="width=device-width, initial-scale=1.0"
</pre>
width of the page will follow screen width of the device
initial-scale will set initial zoom level

Size content to view port :
1. No Horizontal scrolling
2. Adjust content to fit within the width of viewport - no larger fixed width component
3. Content should not replay on particular viewport's width
4. Use media queries to apply styling

media queries:
==============

@media => to include a block of CSS properties only if a certain condition is true

<pre>
eg: @media only screen and (max-width: 500px) {
    body {
        background-color: lightblue;
    }
}
</pre>
Instead of changing styles when the width gets smaller than 768px, we should change the design when the width gets larger than 768px. This will make our design Mobile First
break point for each device

Media queries can also be used to change layout of a page depending on the orientation of the browser.
<pre>
eg; @media only screen and (orientation: landscape) {
    body {
        background-color: lightblue;
    }
}
</pre>
Grid-View
==========
A responsive grid-view often has 12 columns, and has a total width of 100%, and will shrink and expand as you resize the browser window.
<pre>
{box-sizing: border-box;} 
</pre>
Ensures padding and border are included in total width and height of an element


<hr>

Bootstrap
=========

It uses HTML, CSS and jQuery to make responsive web pages

<pre>
Bootstrap														                         
– Bootstrap offers unlimited number of UI elements				  
– Bootstraps uses pixels										                 
– Bootstrap encourages to design for both desktop and mobile.
– Bootstrap support LESS as its preprocessor				
Foundation
– In Foundation UI element options are very limited in numbers
– Foundation use REMs
– Foundation encourages to design mobile first
– Foundation support Sass and Compass as its preprocessor
</pre>

offset
======

.col-md-offset-*

Moves the column to the right,increate the left margin of column by * columns

push and pull 
=============
<pre>
  div class="col-sm-4 col-sm-push-8">.col-sm-4 .col-sm-push-8 /div
  div class="col-sm-8 col-sm-pull-4">.col-sm-8 .col-sm-pull-4 /div
</pre>
Change column ordering

Jumbotron
==========
Big box for calling extra attention to some special content or information.
A jumbotron is displayed as a grey box with rounded corners. It also enlarges the font sizes of the text inside it.
Use a div element with class .jumbotron to create a jumbotron
It can be placed inside a container or outside a container

Page Header
===========
A page header is like a section divider.
The .page-header class adds a horizontal line under the heading (+ adds some extra space around the element).

Pagination
==========
<pre>
.pagination to ul - to include pagination
.disabled - unclickable link
.active - current page
</pre>
breadcrums
==========
Another form of pagination 
.breadcrumb eg <code> Home/ Login/ Register </code>

Wells
=====
The .well class adds a rounded border around an element with a gray background color and some padding

bootstrap text or typography
============================
<pre>
h6 - 12px
h5 - 14px
h4 - 18px
h3 - 24px
h2 - 30px
h1 - 36px

small- lighter secondary text in any heading
mark - highligh a text
abbr
blockquote - .blockquote-reverse to show the right aligned quote
dl descriptionlist
kbd - keyboard inputs
</pre>
two ways to display code
=========================

<pre>
code - display code inline
pre - fixed width font along with space and line breaks
</pre>
contextual colours
==================

<pre>
.text-muted, .text-primary, .text-success, .text-info, .text-warning, and .text-danger
.bg-primary, .bg-success, .bg-info, .bg-warning, and .bg-danger
.lead				Makes a paragraph stand out	
.small				Indicates smaller text (set to 85% of the size of the parent)
.text-left			Indicates left-aligned text	
.text-center		Indicates center-aligned text	
.text-right			Indicates right-aligned text	
.text-justify		Indicates justified text	
.text-nowrap		Indicates no wrap text	
.text-lowercase		Indicates lowercased text	
.text-uppercase		Indicates uppercased text	
.text-capitalize	Indicates capitalized text	
.initialism			Displays the text inside an <abbr> element in a slightly smaller font size
.list-unstyled		Removes the default list-style and left margin on list items (works on both ul and ol). This class only applies to immediate children list items (to remove the default list-style from any nested lists, apply this class to any nested lists as well)	Try it
.list-inline		Places all list items on a single line	
.dl-horizontal		Lines up the terms (dt tag) and descriptions (dd tag) in dl elements side-by-side. Starts off like default dl s, but when the browser window expands, it will line up side-by-side
.pre-scrollable		Makes a pre element scrollable	
</pre>



 
