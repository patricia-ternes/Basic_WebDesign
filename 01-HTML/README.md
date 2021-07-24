<!-- PROJECT LOGO -->
<br />
<p align="center">
    <a href="#important">
        <img src="../inputs/icons/005-html.png" alt="Logo" height="80" id="logo">
    </a>
    <h1 align="center"> Hypertext Markup Language - HTML </h1>
</p>

    
In this page you will find basic informations about HTML.

<a id="important"></a>
## Important

* This repository is under construction!
* <div>Icons made by <a href="https://www.freepik.com" title="Freepik">Freepik</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a></div>

---
---
## Table of Contents
<details open="open" id="toc">
<!-- MarkdownTOC -->

1. [General structure of an HTML page](#general-structure-of-an-html-page)
    1. [Common `body` elements:](#common-body-elements)
    1. [Common `head` elements:](#common-head-elements)
1. [Elements](#elements)
    1. [Headings](#headings)
    1. [Paragraph](#paragraph)
    1. [Comment](#comment)
    1. [Anchor Elements](#anchor-elements)
    1. [Image](#image)
    1. [Unordered List](#unordered-list)
    1. [Ordered List](#ordered-list)
    1. [Division Element](#division-element)
    1. [Layout Elements](#layout-elements)
    1. [Form element](#form-element)
        1. [Text Field](#text-field)

<!-- /MarkdownTOC -->
</details>

aa

<a id="general-structure-of-an-html-page"></a>
## General structure of an HTML page
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

<a id="common-head-elements"></a>
### Common `head` elements:
* title (required)
* style
* meta
* base
* link
* script
* noscript

<a id="elements"></a>
## Elements
Most elements have opening and closing tags. Usually a tag has the following structure:

* Opening tag: `<element>`
* Closing tag: `</element>`

HTML elements can have attributes like:

* `id` attribute: specify a unique id for an HTML element.
* `class` attribute: specify a class (multiple `style` attributes defined in the `head` section or in an external CSS file) for an HTML element.
* `style` *inline* attribute: uses a inline CSS to apply a style for an HTML element.

For example

```html
<h1> This is a heading without attributes. </h1>

<h1 id="main-title" class="red-text" style="font-size:20px"> 
    This is a heading with an id, a class and a style attributes.
</h1>
```

<a id="headings"></a>
### Headings

* Main heading (h1) tag: `<h1>` and `</h1>`
* Subheading (h2) tag: `<h2>` and `</h2>`
* Other heading levels: h3, h4, h5 and h6

For example

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

* Comment tag:  &lt;!-- `<--` and `-->`

```html
<!-- This is a comment -->
```

<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="anchor-elements"></a>
### Anchor Elements
Anchor elements are used to link content to the page.

* Anchor tag: `<a href="url_location">this links to some url</a>`
* href attribute: destination web address

For example, the HTML code
```html
<a href="https://unsplash.com/">this links to Unsplash (source of freely-usable images)</a>
```
Generates the following visualization:
<a href="https://unsplash.com/">this links to Unsplash (source of freely-usable images)</a>

Anchor tags can link contents inside the same page. In this case is necessary:

1. Include an identification attribute (`id`) in the desired element;
2. Use the `href` attribute fallowed by a `#` and the `id` in the `<a>` tag to link the element;

For example, the HTML code
```html
<p id='paragraph-to-link'> This paragraph can be linked internally </p>

<a href="#paragraph-to-link">this links to the previous paragraph.</a>
```
Generates the following visualization:
<p id='paragraphy-to-link'> This paragraph can be linked internally </p>

<a href="#paragraphy-to-link">this links to the previous paragraph.</a>

<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="image"></a>
### Image

* Image tag: `<img src="file/complete/path/or/url" alt="Image description">`
* Image required attributes: `src` (image path) and `alt` (image description).
* Important: image tag is self-closing.
* Image additional attributes: height, width, usemap, style (and others!)

For example, the HTML code

```html
<img src="https://bit.ly/3sNs7V7" alt="Female software engineer with projected code." width="400">
```
Generates the following visualization

<img src="https://bit.ly/3sNs7V7" alt="Female software engineer with projected code." width="400">

*(image from [Unsplash](https://unsplash.com/)).*

<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="unordered-list"></a>
### Unordered List
* Unordered list tag: `<ul>` and `</ul>`
* List item tag: `<li>` and `<\li>`

For example, the HTML code
```html
<ul>
    <li>first item</li>
    <li>second item</li>
    <li>last item</li>
</ul>
```
Generates the following visualization:
<ul>
    <li>first item</li>
    <li>second item</li>
    <li>last item</li>
</ul>

<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="ordered-list"></a>
### Ordered List
* Ordered list tag: `<ol>` and `</ol>`
* List item tag: `<li>` and `<\li>`

For example, the HTML code
```html
<ol>
    <li>first item</li>
    <li>second item</li>
    <li>last item</li>
</ol>
```
Generates the following visualization:
<ol>
    <li>first item</li>
    <li>second item</li>
    <li>last item</li>
</ol>

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

<!-- para criar formularios
<br/><br/><br/>
<a href="#logo"> *Back to top* </a>

<a id="form-element"></a>
### Form element
<a id="text-field"></a>
#### Text Field
* Text field tag: `<input type="text">`
* Placeholder atribute: text to display in the text field element.
* Important: text fild is self-closing.

For example, the HTML code
```html
<input type="text" placeholder="type your name">
```
Generates the following visualization:
<input type="text" placeholder="type your name">
-->


<!--
For example, the HTML code
```html
<h1>Lorem ipsum dolor</h1>

<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur commodo bibendum odio id ullamcorper. Pellentesque vel velit et ipsum consectetur porta. In hac habitasse platea dictumst. Nulla condimentum mi ac purus pellentesque pharetra. Vivamus bibendum mi magna, nec ornare eros ultricies sed. Nam a est a leo dapibus posuere. Donec aliquam tristique leo eu consequat. Phasellus sagittis nec nisi id bibendum.</p>

<h2>Ut vel odio</h2>

<p>Donec nisl elit, malesuada nec nisi nec, lobortis eleifend purus. Nullam auctor enim id nibh vulputate blandit. Quisque purus ligula, commodo et mi vel, euismod eleifend urna. Morbi et purus vitae tellus pharetra dignissim et eu nisi. In lobortis ligula id quam euismod blandit. Quisque aliquet auctor leo, in aliquet velit varius vel. Phasellus urna lectus, viverra at eleifend sit amet, tincidunt at eros. Vestibulum vitae pulvinar lorem. Proin lectus lectus, placerat id nunc sit amet, tristique aliquet neque. Aenean sit amet aliquam magna. Mauris non viverra ligula. Nullam at accumsan quam. Sed sed est sapien.</p>
```
Generates the following visualization

<div>
    <h1 style="color: blue;">Lorem ipsum dolor</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur commodo bibendum odio id ullamcorper. Pellentesque vel velit et ipsum consectetur porta. In hac habitasse platea dictumst. Nulla condimentum mi ac purus pellentesque pharetra. Vivamus bibendum mi magna, nec ornare eros ultricies sed. Nam a est a leo dapibus posuere. Donec aliquam tristique leo eu consequat. Phasellus sagittis nec nisi id bibendum.</p>
    <h2>Ut vel odio</h2>
    <p>Donec nisl elit, malesuada nec nisi nec, lobortis eleifend purus. Nullam auctor enim id nibh vulputate blandit. Quisque purus ligula, commodo et mi vel, euismod eleifend urna. Morbi et purus vitae tellus pharetra dignissim et eu nisi. In lobortis ligula id quam euismod blandit. Quisque aliquet auctor leo, in aliquet velit varius vel. Phasellus urna lectus, viverra at eleifend sit amet, tincidunt at eros. Vestibulum vitae pulvinar lorem. Proin lectus lectus, placerat id nunc sit amet, tristique aliquet neque. Aenean sit amet aliquam magna. Mauris non viverra ligula. Nullam at accumsan quam. Sed sed est sapien.</p>
</div>
-->