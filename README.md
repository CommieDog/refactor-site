# Refactor Website for Accessibility

## Introduction 

This project was undertaken for a marketing agency client who wanted to refactor their website codebase to meet basic accessibility standards. The client wanted the basic look-and-feel of the website unchanged; the changes made "under the hood" aimed to perserve the website for unimpared human users while being more accessible to impared users and search engines.

![The Horiseon webpage includes a navigation bar, a header image, and cards with text and images at the bottom of the page.](./Assets/website-mockup.png)

A sample deployment of the website is available on [GitHub Pages](A).

## Table of Contents

If your README is very long, add a table of contents to make it easy for users to find what they need.

* [Description](#description)
* [Features](#features)
* [Future Work](#future-work)
* [License](#license)


## Description

A substantial portion of the work involved adding semantic HTML to the webpage. The final product makes use of several semantic HTML elements such as `<header>`, `<footer>`, and `<section>`. Elements within sections were reordered in a logical fashion, while their layouts were modified to match the original layout of the webpage via CSS properties. Header elements were reclassified to match good practice and images were given alternate descriptors. Finally, a refactoring of the webpage's CSS file was undertaken, simplifying selector criteria and adding comments.


## Features

* Addition of `<title>` element
* Proper use of semantic HTML
    * Added `<header>` element, complete with included `<nav>` element
    * Added `<main>` element
    * Replaced nonsemantic `<div>` elements with `<section>`
    * Wrapped images in `<figure>`
    * Added `<footer>` element
* Logical ordering of content within both the Service and Benefit subsections
* Proper numbering for header elements
* Images with alternate descriptors
* Extensive use of CSS positioning properties, such as `float`, `display`, and `position`, to display content


## Future Work

Future work on this project would likely come in the form of improved accessibility, partucularly for users with small screen sizes. The basic layout of the webpage is not stable when squeezed into small sizes, and a few visual elements are too indistinct even for nonimpared users to notice. The Benefits section in particular would benefit from the use of flexboxes.


## License

© 2022 John Netzel. All Rights Reserved.