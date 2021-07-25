<!-- PROJECT LOGO -->
<br />
<p align="center">
    <a href="#important">
        <img src="../inputs/icons/002-css.png" alt="Logo" height="80" id="logo">
    </a>
    <h1 align="center"> Cascading Style Sheets</h1>
</p>

## General Information
In this page you will find basic informations about CSS.

## Important

This repository is under construction!

## Introduction

CSS provide to the web browser instructions about how a HTML code should be displayed.

Common instructions are related with:

* Fonts: colour, font size, font families
* Text: alignment, decoration, spacing
* Borders: width, colour, rounded
* Margins and Paddings


CSS can be used in 3 ways:

* **Inline**: `style` attribute in HTML elements
* **Internal**: `<style>` element in the `<head>` section
* **External**: external CSS file add through `<link>` element


## Colour

The most common style attribute. HTML colours can be referenced by:

* [Colour name](https://www.w3schools.com/colors/colors_names.asp): `violet`
* [RGB color values](https://www.w3schools.com/colors/colors_rgb.asp): `rgb(238, 130, 238)`
* [Hexadecimal color values](https://www.w3schools.com/colors/colors_hexadecimal.asp): `#EE81EE`
* [HSL (hue, saturation, lightness)](https://www.w3schools.com/colors/colors_hsl.asp): `hsl(300, 76%, 72%)`

Different attributes uses colour value:

* Text colour: `color: violet;`
* Border colour: `border-color: hsl(300, 76%, 72%);`
* Background colour: `background-color: rgb(238, 129, 238);`

## Font

### Generic font families

Font names are divided in five font families. The generic family names: are

* cursive
* fantasy
* monospace
* sans-serif
* serif

```css
font-family: cursive;
```

### External font

Several places provide additional fonts. For example, you can use the [Google Fonts](https://fonts.google.com/) to find a free font.

To use the external font it is necessary to:

1. Import the desired font using a `link` element. Usually the external source provides the correct link to use.
2. Set the `font-family` attribute

For example, for the [*Bad Script*](https://fonts.google.com/specimen/Bad+Script?preview.text_type=custom) font:
```css
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Bad+Script" rel="stylesheet">
```
```css
font-family: "Bad Script"
```

### Universal fonts

Some fonts are (**probably**) installed in all browsers and devices. So it is possible to use them without import external information.

Bellow is listed one font for each font family:

* cursive: Brush Script MT
* fantasy: (?)
* monospace: Courier New
* sans-serif: Arial
* serif: Times New Roman

```css
font-family: "Courier New";
```

### Font Degrade
Sometimes the font can not be used by the browser (even the *universal fonts*), so it is recommended to provide other possibilities to the browser know what to do in this case. The last font should be a generic one.
```css
font-family: "Bad Script", "Brush Script MT", cursive;
```

### Font size

Attribute to set the font size. Can be set in different ways:

* Pixel: `font-size: 40px;`
* Em: `font-size: 2.5em;`
    * Default size: `1em = 16px`, so `2.5em = 40px`.
* Viewport width (vw): `font-size:10vw;`
    * `100vw = 100%` of viewport width


## CSS Selectors
To understand how to select and change the style in different ways, consider the following HTML small code:

```html
<h2 id="first-heading" class="centre"> First title</h2>

<h2 id="second-heading"  class="centre-blue"> Second title</h2>

<h2 id="third-heading"  class="centre-blue"> Third title</h2>

<p class="centre"> This is a paragraph </p>
```

This code has three titles with the same importance level in the text, so all three have the same `element` value. Each title has a specific `id`. The second and the third title have the same `class`, but the first has a unique `class`.


### Element Selector
Used to apply one style for a specific element. All entry of this element will receive this style. The general format is:
```css
element {
    attribute: value;
}
```

For example, to apply a red colour in all `<h2>` heading text.
```css
h2 {
    color: red;
}
```

For example, to apply a blue colour in all `<p>` text.
```css
p {
    color: blue;
}
``` 

#### `id` Selector
Used to select just the element set with the same `id`. The general format is (note the `#`):
```css
#id-name {
    attribute: value;
}
```

For example, to apply a red colour only in the second `<h2>` heading:
```css
#second-heading {
    color: red;
}
```

#### `class` Selector
Used to select all elements set with the same `class`. The general format is (note the `.`):
```css
.class-name {
    attribute: value;
}
```

For example, to apply a blue colour and to centralize the second and third titles:
```css
.centre-blue {
    text-align: center;
    color: blue;
}
```

For example, to centralize the first title and the paragraph:
```css
.centre {
    text-align: center;
}
```


#### `*` Universal Selector
Used to select and apply the same style to all elements. For example, to apply a blue colour and to centralize all titles and the paragraph:

```css
* {
    text-align: center;
    color: blue;
}
```

#### Grouping Selector
Used to set the same style to different elements. For example:
```css
h2, p {
    text-align: center;
    color: blue;
}
```

#### Nested Selector
Used to set one style for the element that has a combination of identification. For example, if the element is `<h2>` and the class is `centre-blue`, than the text should be violet and centralized.

```css
h2.centre-blue{
    color:violet
    text-align: center;
}
```
This code affect the second and the third titles. Other example:
```css
h2.centre{
    color:violet
    text-align: center;
}
```
This code affect just the first title, even if the paragraph has the same class.