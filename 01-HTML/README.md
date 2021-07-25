<!-- PROJECT LOGO -->
<br />
<p align="center">
    <a href="#important">
        <img src="../inputs/icons/005-html.png" alt="Logo" height="80" id="logo">
    </a>
    <h1 align="center"> Hypertext Markup Language</h1>
</p>

    
In this page you will find basic informations about Hypertext Markup Language (HTML).

<a id="important"></a>
**Important**

* This repository is under construction!
* <div>Icons made by <a href="https://www.freepik.com" title="Freepik">Freepik</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a></div>


---

<details open="open" id="toc">
    <summary>Table of Contents</summary>
<!-- MarkdownTOC -->

- [General structure of an HTML page](#general-structure-of-an-html-page)
- [Basic elements structure](#basic-elements-structure)
    - [Common `body` elements:](#common-body-elements)
- [Headings](#headings)
    - [Paragraph](#paragraph)
    - [Comment](#comment)
    - [Anchor Elements](#anchor-elements)
    - [Image](#image)
    - [Unordered List](#unordered-list)
    - [Ordered List](#ordered-list)
    - [Division Element](#division-element)
    - [Layout Elements](#layout-elements)
- [Common `head` elements:](#common-head-elements)

<!-- /MarkdownTOC -->
</details>

<a id="general-structure-of-an-html-page"></a>
## General structure of an HTML page

* `<!DOCTYPE>` : define the HTML version
    * self closing tag
    * `<!DOCTYPE html>`: for HTML5
* html: root element
    * tag: `<html>` and `</html>`
* head: meta information
    * tag: `<head>` and `</head>` 
* body: container for visible information
    * tag: `<body>` and `</body>`

```html
<!DOCTYPE html>
<html>
  
  <head>
    Information about the HTML page should be placed within a head tag.
  </head>

  <body>
    The content displayed for a user of the HTML page should be placed within a body tag.
  </body>

</html>
```
<a id="basic-elements-structure"></a>
## Basic elements structure
Most HTML elements have opening and closing tags. Usually a tag has the following structure:

* Opening tag: `<element>`
* Closing tag: `</element>`

HTML elements can have attributes like:

* `id` attribute: specify a unique id for an HTML element.
* `class` attribute: specify a class (multiple `style` attributes defined in the `head` section or in an external CSS file) for an HTML element.
* `style` *inline* attribute: uses a inline CSS to apply a style for an HTML element.

```html
<h1> This is a heading without attributes. </h1>

<h1 id="main-title" class="red-text" style="font-size:20px"> 
    This is a heading with an id, a class and a style attributes.
</h1>
```

<a id="common-body-elements"></a>
### Common `body` elements:
* [headings](#headings)
* [paragraph](#paragraph)
* [comment](#comment)
* [anchor](#anchor-elements)
* [image](#image)
* [unordered list](#unordered-list)
* [ordered list](#ordered-list)
* [division](#division-element)
* [header, main, footer, and sections](#layout-elements)
* form, input, radio, and checkbox

<a id="headings"></a>
## Headings

* Main heading (h1) tag: `<h1>` and `</h1>`
* Subheading (h2) tag: `<h2>` and `</h2>`
* Other heading levels: h3, h4, h5 and h6


```html
<h1> This is a main heading </h1>

<h2> This is a subheading </h2>
```


<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="paragraph"></a>
### Paragraph

* Paragraph tag: `<p>` and `</p>`

```html
<p> This is a paragraph </p>
```

<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="comment"></a>
### Comment

* Comment tag: `<--` and `-->`

```html
<!-- This is a comment -->
```

<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="anchor-elements"></a>
### Anchor Elements
Anchor elements are used to link content to the page.

* Anchor tag: `<a href="url_location">`  and `</a>`
* `href` attribute: destination address

```html
<a href="https://github.com/">this text links to GitHub</a>
```

* Anchor tags can link contents inside the same page. In this case is necessary:

    1. Include an identification attribute (`id`) in the desired element;
    2. Use the `href` attribute fallowed by a `#` and the `id` in the `<a>` tag to link the element;

```html
<p id='paragraph-to-link'> This paragraph can be linked internally </p>

<a href="#paragraph-to-link">this links to the previous paragraph.</a>
```

<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="image"></a>
### Image

* Image tag: `<img src="file/complete/path/or/url" alt="Image description">`
* Image required attributes: `src` (image path or url) and `alt` (image description).
* Important: image tag is self-closing.
* Image additional attributes: height, width, usemap, style (and others!)

```html
<img src="../inputs/icons/005-html.png" alt="Logo" height="80" id="logo">
```


<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="unordered-list"></a>
### Unordered List
* Unordered list tag: `<ul>` and `</ul>`
* List item tag: `<li>` and `<\li>`

```html
<ul>
    <li>first item</li>
    <li>second item</li>
    <li>last item</li>
</ul>
```

<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="ordered-list"></a>
### Ordered List
* Ordered list tag: `<ol>` and `</ol>`
* List item tag: `<li>` and `<\li>`

```html
<ol>
    <li>first item</li>
    <li>second item</li>
    <li>last item</li>
</ol>
```

<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="division-element"></a>
### Division Element

Division tags are used to nest different HTML elements in just one container.

* Division tag: `<div>` and `</div>`

For example, the HTML code
```html
<div id="ordered-list">   
    <ol>
        <li>first item</li>
        <li>second item</li>
        <li>last item</li>
    </ol>
</div>
```
Generates the following visualization:
<div>  
    <ol>
        <li>first item</li>
        <li>second item</li>
        <li>last item</li>
    </ol>
</div>

Note that in terms of visualization, the `div` tag has not changed anything. The purpose of the tag is to improve the code's readability and to allow future style improvements.

<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="layout-elements"></a>
### Layout Elements
To further improve the code's readability, is recommended that each HTML body be divided into 3 parts: header, main, and footer.

* Main tag: `<main>` and `</main>`
* Header tag: `<header>` and `</header>`
* Footer tag: `<footer>` and `</footer>`

The basic `body` code:
```html
<body>
    <header>
        Header content. This tag replace the <div class="header"> tag.
    </header>
    <main>
        The main content of the HTML page should be placed within a main tag.
    </main>
    <footer>
        Footer content. This tag replace the <div class="footer"> tag.
    </footer>
</body>
```

There are others semantics elements to define different parts of the HTML: `article`, `aside`, `details`, `figcaption`, `figure`, `footer`, `header`, `main`, `mark`, `nav`, `section`, `summary`, `time`. These elements are organized as outlined in the image (*from [w3schools](https://www.w3schools.com/html/html5_semantic_elements.asp)*) below.

<a href="https://www.w3schools.com/html/html5_semantic_elements.asp"><img src="https://www.w3schools.com/html/img_sem_elements.gif" alt="HTML Semantics elements. Image from w3schools site" style="width: 50px;"></a>

You can find detailed information about HTML Semantics in the [w3schools](https://www.w3schools.com/html/html5_semantic_elements.asp) site.

<a id="common-head-elements"></a>
## Common `head` elements:
* title (required)
* style
* meta
* base
* link
* script
* noscript
