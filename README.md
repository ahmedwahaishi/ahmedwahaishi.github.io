# Project 0
Web Programming with Python and JavaScript

Important Notes:
- Please test my website using Google Chrome.




My Personal website's Project contains 4 pages:
==============================================
- index.html:
     (reached through (Home) navigation)
- About.html:
     (reached through (About) navigation).
- Resume.HTML:
    (reached through (Resume) navigation and also by clicking (Tell me more) button in the index's home page) .
- Folio.html:
    (reached through (AhmedFolio) navigation)



===============================================================================================
Each page contains 3 main parts except index contains 4 parts:
==============================================================
- Navigation Bar. (Same content is Repeated for all pages)
- (Only Index Page) has Header Part.
- Middle part.
- Footer Part (For contact & info) Same content is Repeated for all pages.


Page Parts Description:
======================


The Navigation Part:
====================

A standard green horizontal responsive navigation bar that becomes vertical on small screens. It is created with the .navbar class, followed by a responsive collapsing class: .navbar-expand-md.
Navbars come with built-in support for a handful of sub-components such navbar-brand for your company or product Name.
The (Toggle button) for the collapsed menu (navbar-toggler):
 collapse JavaScript plugin is used to show and hide content. The Button is used as trigger that is mapped to specific elements you toggle. Collapsing an element will animate the height from its current value to 0. Given how CSS handles animations
The Menu Items:
I used the class navbar-nav for the list element that holds the menu.
To add links inside the navbar by using a <ul> element with class="navbar-nav". Then add <li> elements with a .nav-item class followed by an <a> element with a .nav-link class.



The Header Part:
===============

I Used page-header class to highlight some special piece of my personal information and to focus on visitor's attention. I also used -fluid to make my container stretches across the width of the screen.
I put a full-screen background image for my landing page header. So I used some jQuery to make the image stretch across the screen with some CSS code as shown below:

In HTML pages:
-------------
<script src="main.js"></script>

In myJS.js:
-----------
$(document).ready(function(){
	$('.header').height($(window).height());
})

In mySheet.css:
---------------
.header {
  background-image: url('images/header-background.jpg');
  background-size: cover;
  background-position: center;
  position: relative;
}



- Middle part:
==============

 - In all pages, I used Bootstrap's classes to divide and control the containers, rows, columns and its built-in features.

 - In (Resume.html), I used the simple way to create table ,order and unorder lists with the header's style tag to control the CSS in the same file.
 I divided the middle part here into two columns:
   1- First column for (Experience Table + Career Summary).
   2- Second column for the (Main Skills).

- In About.html), I divided the middle part here into two columns:
  1- First column for (About Summary).
  2- Second column for the (My Photo).

- In (Folio.html) & (Index.html), I used 4 columns including:
  1-Three columns for ( 3 photos and 3 paragraphs).
  2- One Column for input form.


- Footer Part:
==============
 - I used page-footer class with container, row, and two columns:
    1- First Column for Additional Information.
    2- Second Column for contact information.

--------------------------------------------------------------------------------------------
I inserted the below lines in each page's beginning:
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="bootstrap/css/bootstrap.min.css">
<link rel="stylesheet" type="text/css" href="mySheet.css">

I inserted the below lines in each page's end:
<script src="jquery-3.3.1.min.js"></script>
<script src="bootstrap/js/bootstrap.min.js"></script>
<script src="myJS.js"></script>

===============================================================================================

I tried to apply all the requirements that you have mentioned below:
====================================================================


•	Your website must contain at least four different .html pages, and it should be possible to get from any page on your website to any other page by following one or more hyperlinks.
-----------------------------------------------------------------------------------------
•	(In Resume Page) Your website must include at least one list (ordered or unordered), at least one table,
-----------------------------------------------------------------------------------------
and
(In Index, About and Folio pages)  at least one image .
-----------------------------------------------------------------------------------------
•	(mySheet.css) Your website must have at least one stylesheet file.
-----------------------------------------------------------------------------------------
•	(In mySheet.css) Your stylesheet(s) must use at least five different CSS properties:
-----------------------------------------------------------------------------------------
and
(In mySheet.css) at least five different types of CSS selectors:
/*-- CSS selectors --*/
.countryCode::before {
     content: "+967 - ";
 }
.selectHDesc::selection {
    color: green;
    background-color: white;
}
.nav-link:hover {
  color: #000;
}
.description p {
  color: #fff;
  font-size: 1.2rem;
  line-height: 1.5;
}
.resumeTitle, .aboutTitle, .aboutSubTitle {
  font-family:Times;
  color: green;
  font-weight: bold;
}


 - (In mySheet.css) You must use the #id selector at least once, and the .class selector at least once:
 .navbar {
   background:#6ab446;
 }

-----------------------------------------------------------------------------------------

•	Your stylesheet(s) must include at least one mobile-responsive @media query, such that something about the styling changes for smaller screens.
@media (max-width: 575.98px) {
  .description {
    left: 0;
    padding: 0 15px;
    position: absolute;
    top: 10%;
    transform: none;
    text-align: center;
  }
  .features {
    margin: 0;
  }
}

-----------------------------------------------------------------------------------------

•	(In all Pages) You must use Bootstrap 4 on your website, taking advantage of at least one Bootstrap component, and using at least two Bootstrap columns for layout purposes using Bootstrap’s grid model.

-----------------------------------------------------------------------------------------

•	Your stylesheets must use at least one SCSS variable, at least one example of SCSS nesting, and at least one use of SCSS inheritance.
/*-- SCSS inheritance  --*/
%titlex{
  font-family:Times;
  color: green;
  font-weight: bold;
}
.aboutTitle {
    @extend %titlex;
    font-size: 50px;
}
.resumeTitle {
    @extend %titlex;
    font-size: 49px;
}
.aboutSubTitle {
  @extend %titlex;
    font-size: 30px;
    color: black;
}
/*-- SCSS Variables to control colors --*/
$colorL01: #6ab446;
$colorL02: #fff;
$colorHover: #000;

/*-- SCSS Nested  --*/
.nav-link {
	color: $colorL02;
	cursor: pointer;
	margin-right: 1em !important;
	&:hover {
		color: $colorHover;
	}
}

-----------------------------------------------------------------------------------------

•	In README.md, include a short writeup describing your project, what’s contained in each file, and (optionally) any other additional information the staff should know about your project.

I used a standard green horizontal responsive navigation bar that becomes vertical on small screens. It is created with the .navbar class, followed by a responsive collapsing class: .navbar-expand-md.
The Header (Page Content Container):
I Used page-header class to highlight some special piece of my personal information and to focus on visitor's attention. I also used -fluid to make my container stretches across the width of the screen.
---------------------------------------------------------------------------------------
In The Header (Page Content Container):
I put a full-screen background image for my landing page header. So I used some jQuery to make the image stretch across the screen with some CSS code as shown below:
Inserted in HTML pages:
<script src="main.js"></script>
In myJS.js:
$(document).ready(function(){
	$('.header').height($(window).height());
})
 And in mySheet.css:
.header {
  background-image: url('images/header-background.jpg');
  background-size: cover;
  background-position: center;
  position: relative;
}


-----------------------------------------------------------------------------------------

Thanks for reading and reviewing my project.
I hope it is OK.
