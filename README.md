# Refactor Website for Accessibility

## Introduction 

This project was undertaken for a marketing agency client who wanted to refactor their website codebase to meet basic accessibility standards. The client wanted the basic look-and-feel of the website unchanged; the changes made "under the hood" aimed to perserve the website for unimpared human users while being more accessible to impared users and search engines.

![The Horiseon webpage includes a navigation bar, a header image, and cards with text and images at the bottom of the page.](https://github.com/CommieDog/refactor-site/blob/main/assets/website-mockup.png)

A sample deployment of the website is available on [GitHub Pages](https://commiedog.github.io/refactor-site/).


## Table of Contents

* [Description](#description)
* [Features](#features)
* [Future Work](#future-work)
* [License](#license)


## Description

A substantial portion of the work involved adding semantic HTML to the webpage. The final product makes use of several semantic HTML elements such as `<header>`, `<footer>`, and `<section>`. Elements within sections were reordered in a logical fashion, while their layouts were modified to match the original layout of the webpage via CSS properties. Header elements were reclassified to match good practice and images were given alternate descriptors. Finally, a refactoring of the webpage's CSS file was undertaken, simplifying selector criteria and adding comments.

### Sample of HTML Refactoring
#### Before
```HTML
<div class="search-engine-optimization">
    <img src="./assets/images/search-engine-optimization.jpg" class="float-left" />
    <h2>Search Engine Optimization</h2>
    <p>
        The dominance of mobile internet use means that users are searching for the right business as they travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase your visibility and find the right customers for your business.
    </p>
</div>
```
#### After
```HTML
<section id="search-engine-optimization" class="service image-on-left">
    <h2>Search Engine Optimization</h2>
    <p>
        The dominance of mobile internet use means that users are searching for the right business as they travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase your visibility and find the right customers for your business.
    </p>
    <figure>
        <img src="./assets/images/search-engine-optimization.jpg" alt="Search engine optimization diagram on notebook"/>
    </figure>
</section>
```


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


## Technologies Used

* HTML
* CSS


## Future Work

Future work on this project would likely come in the form of improved accessibility, partucularly for users with small screen sizes. The basic layout of the webpage is not stable when squeezed into small sizes, and a few visual elements are too indistinct even for nonimpared users to notice. The Benefits section in particular would benefit from the use of flexboxes.


## License

© 2022 John Netzel. All Rights Reserved.