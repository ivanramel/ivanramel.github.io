---
layout: essay
type: essay
title: "It's frameworking' time!"
# All dates must be YYYY-MM-DD format!
date: 27 Feb 2025
published: true
labels:
 - UI Frameworks
 - Bootstrap
---

<!--rounded float-start pe-4-->

<p align="left">
<img width="200px" class="float-start pe-4" src="../img/Bootstrap_logo.png">
</p>

## Why bother with framework?

Since we learned HTML and CSS to help us build static web pages, why would we need to learn a framework? Wouldn’t it be better to invest our time into learning more about HTML and CSS? With enough time, we can create everything that a framework already contains such as navbar, forms, buttons, etc. Well, that’s **The Thing**:

<p align="center">
<img width="400px" src="../img/The_Thing_HeroPortrait.png">
</p>

We could make it, but why waste our time when it’s already provided by a framework? This is especially apparent when we have to make all these elements for a webpage—it becomes hard to keep track of everything and maintain a consistent design across the site. Frameworks also make the code easier to maintain in the long run. That said, many frameworks can feel like learning an entirely new language, which is overwhelming. So where do we start?

## Bootstrap: Making sense of all of this

Out of all the frameworks we probably haven’t touched or heard about yet, why use **Bootstrap**?

For one, it seems to be a more beginner-friendly option for people like us who just learned basic HTML and CSS. It comes with pre-made components like buttons, forms, navbars, etc. And we’re not restricted to the default designs, either. You can customize many Bootstrap elements directly from the HTML file. For example, when you assign a class to a component, you can use Bootstrap utility classes to control margins, padding, alignment, and more—without needing to write a single line of CSS.

If your design needs go beyond that, you can always modify the CSS file manually. What I’m trying to say is: Bootstrap gives you the ingredients to cook with, but you’re still the chef.

## My Experience with Bootstrap

So far, I’ve made three web pages with Bootstrap: **Island Snow**, **Gyu-Kaku**, and **Murphy’s Bar and Grill**.

I started with Island Snow as part of an assignment designed to get us comfortable using Bootstrap’s toolset. We practiced building navbars and working with the grid system. The entire page was built using only Bootstrap classes inside the HTML file—from customizing text and background colors to structuring the navbar and footer. I didn’t even need to touch the CSS file because the design was relatively simple.

<p align="center">
<img width="700px" src="../img/island-snow-screenshot.png">
</p>

The next webpage, **Gyu-Kaku**, was based on our choice to recreate any site, assuming it didn’t already use Bootstrap. I chose Gyu-Kaku because I was hungry—and the website looked clean and simple.

Initially, I was confident. But I quickly ran into problems trying to match the original design exactly. For starters, I wasted time trying to use the same fonts, only to find out they weren’t open source or available via Google Fonts. Then I made another mistake: I tried building the navbar without referring to Bootstrap’s documentation. I thought I could wing it.

That led to issues like:
- The navbar not scaling with window size
- It failing to collapse into a mobile-friendly dropdown
- Layout inconsistencies across devices

Although I completed the project, those problems remained. In hindsight, ignoring the documentation was a big mistake. Just like with coding in general, we should **expect users to do things we didn’t plan for**, and design accordingly.


<p align="center">
<img width="700px" src="../img/gyu-kaku-yourchoice-screenshot.png">
</p>

Unfortunately, I repeated the same mistakes in my **Murphy’s Bar and Grill** webpage. Again, the navbar and footer didn’t span the full width of the page. Their edges didn’t touch the sides of the screen, which broke the look of the layout.

These issues stemmed from not properly using Bootstrap’s grid system and container classes. Had I taken time to better understand how Bootstrap structures rows and columns—or checked the docs—this wouldn’t have happened.

## Conclusion

Frameworks are—and will continue to be—essential tools in web development. They **save time**, **enforce consistent design**, and **remain highly customizable**.

Bootstrap, in particular, makes it easy to:
- Build responsive components
- Quickly layout content with a grid system
- Maintain design uniformity without extensive CSS

But like anything worthwhile, using frameworks properly takes time and effort. At first, they can seem intimidating and even restrictive. But once you understand how to work with them—not against them—they become second nature, like your favorite programming language.
