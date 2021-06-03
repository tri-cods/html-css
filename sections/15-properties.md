[<<<Back](14-classes.md) | [Next>>>](16-creating_stylesheet.md)

# CSS Properties

Below is a list of useful properties that can be modified with CSS. There are also [CSS cheatsheets](https://courses.cs.washington.edu/courses/cse154/15sp/cheat-sheets/css-cheat-sheet.pdf) available online.

## Color

Modern browsers recognize the names of 140 common colors: you can find a full [list of color names here](https://htmlcolorcodes.com/color-names/). To set text color to a standard blue, for example, you'd add `color: blue;` inside the declaration for that element. Beyond those common names, you can also identify colors by their hexadecimal (or simply 'hex') values, which you can look up using a color picker or [hex calculator](https://www.w3schools.com/colors/colors_hexadecimal.asp). [This tutorial](https://www.w3schools.com/colors/default.asp) provides a more in-depth discussion of colors in css.

The **color** property sets the color of an element:

```css
p {
  color: #000000;
}
```

The **background color** property sets the background color of an element:


```css
p {
  background-color: pink;
}
```

## Alignment

**Text align** aligns an element to the left, center, or right.

```css
text-align: center;
```

**Padding**: sets the space between text and the "box" (`<div>` or other element) surrounding it.

```css
padding: 10px;
padding-right: 10px
```

**Margin**: sets the space between an element's box and the next element (or the edge of the page).

```css
margin: 10px;
margin-top: 10px;
```

## Width and height

Sets the **width** or **height** of an element, usually the value is either a percentage of its container or a number of pixels:  

```css
width: 50%;
height: 40px;
```

## Other values

**Float** determines if an element appears next to another element (and on which side) - for example, you could use `float: left;` to make an image sit in-line with a text element on the left side. [Learn more about float here](https://www.w3schools.com/css/css_float.asp)

**Display** determines if an element is treated as an inline element or a 'block' on a new line. If you set display to `none`, an element will not be visible on the page.

```css
display: inline;
display: block;
display: none;
```

**List style** determines the type of marker or 'bullet' accompanies list items. To get rid of the markers, use `list-style-type: none;` 

**Font family** sets the font of a text. Because not all browsers support all fonts, it's a good idea to include the name of a specific font (such as 'Arial'), a 'fallback' font in case that font doesn't display, and the family the font belongs to ('sans-serif').

```css
font-family: "Times New Roman", Times, serif;
```

If you want to get fancy, you can import web fonts from a repository such as [Google Fonts](https://fonts.google.com/).


[<<<Back](14-classes.md) | [Next>>>](16-creating_stylesheet.md)
