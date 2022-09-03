# TechClub-International
A generic website for a technical/programming club.

# Website link
https://ritamdasgupta.github.io/TechClub-International/


Figma Design Template Link:
https://www.figma.com/file/4Ipcc3NaSCtuhouiLxeq0T/DEVCLUB_WEBSITE?node-id=0%3A1


# Introduction
This website has been made using Bootstrap 5, which I imported locally. CSS is mostly inline, and a few lines have been included internally with comments.
The basic design template for the website has also been provided, which i made using Figma. However, during implementation, i learnt about numerous Bootstrap functionalities such as carousels, popovers, accordions and cards, and accordingly included them in my webpage.
So, there are some differences present between my Figma template and final submission.
The site consists of 7 pages- 
1) Landing page (Home)
2) Projects
3) Resources
4) Events
5) Team
6) Blogs
7) Contacts and Footer
 
# Home
I made a logo (using Figma) for TechClub-International too, and it has been included in the navbar on the top-left corner.
The navbar is functional. I used a sticky navbar since each page of the site contains only a small amount of content, and it seemed better to me to allow scrolling. 
Further, a search bar has been provided along with the navbar. However, I only did the front-end work, so the bar is not functional. I did want to do the back-end work, use PHP and make it functional, but could not manage to do so before the deadline.
An animation has been made for the "Welcome" text using CSS keyframes.

# Projects
Used Bootstrap grids for this. The enlarge-on-hover effect was added with CSS. I faced significant problems aligning the grid to the centre of the screen. My initial solution was to place each image of each cell in a container and then pad it. This worked fine, but the downside was that the images did not stack over each other in smaller screens. 
I finally managed to make it responsive by using the "justify-content-center" command in the "row" class (this was mentioned on Stack Overflow), and implemented this instead of my previous solution.
To enhance the user experience, popovers have been added to each image which trigger on cursor hover. "Popper.js", the 3rd-party library for popovers, is included under bootstrap.bundle.min.js
All the projects have working links, to various github repos i found interesting.

# Resources
Although my initial idea (as can be seen from the Figma file) was to use the same format for this page as for "Projects", I found it a bit repetitive. While going through the IITD DevClub site, I saw that accordions were used for this purpose, a format I liked. So i borrowed this format and made my page in the same way. The links are functional and point to WnCC(IIT Bombay) resources.
The only problem I faced here was that the accordion, when fully opened, extended beyond the background image. My attempt to fix this was to put the entire accordion object inside a container, and have the background as a parent element to this container.  I also made the background image itself larger (putting "height:150vh" in the style attribute). This ensured that the background image was large enough to cover the entire accordion in my desktop. However, I noticed this did not work on my phone. Later in my final submission i removed the height specification for background to let Bootstrap automatically adjust it, and instead added some line breaks to make my page larger. This final solution worked on all devices i tested.

# Events
I found documentation about carousels on [www.getbootstrap.com](https://getbootstrap.com/docs/5.2/components/carousel/), which i found interesting and decided to implement it. This page did not give me any significant problems. The picture dimensions might be a bit off depending upon screen dimensions, but i think that is not an implementation fault, just that the picture dimensions do not match the screen. This page seems to render better on mobile phones than the desktop. I again used WnCC material for content, as posters for DevClub events seemed unavailable.

# Team
Decided to use cards for this. This renders fine on all devices i tested too. Used buttons for the "View Profile", which all link to different DevClub seniors, except one :). Aligned the cards using a Bootstrap grid.

# Blogs
Reused the same format as the Projects page for this (no, not running out of ideas). The links are functional.

# Contacts and Footer
Used Bootstrap forms to create the contact form. Did only the front-end work for this, so the form is not functional. From what i read on various sites making it functional would involve creating a SQL database and using PHP to link server and client. But i did not find time to implement this.
Added a footer too for aesthetics.


# Citations
I used numerous resources and learnt many things while doing this assignment. Here are a few citations:

1) https://getbootstrap.com/
2) https://www.w3schools.com/html
3) https://www.stackoverflow.com/

These three form the bulk of my browser history over the past few days. ALmost all of my research happened via these sites. I also used www.tutorialrepublic.com and www.youtube.com occasionally.
For content i heavily relied on www.wncc-iitb.org and https://devclub.in/#/.
I used www.unsplash.com for photos and background images.

# Tests
I tested the mobile-friendliness of the website on https://search.google.com/test/mobile-friendly, and it passed. I also tested on various devices I have including tablets, laptop and a mobile phone and it appears responsive.
