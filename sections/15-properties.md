[<<<Back](14-classes.md) | [Next>>>](16-creating_stylesheet.md)

# CSS Properties

Below is a list of useful properties that can be modified with CSS -- there are many, many more! This [CSS Tutorial from W3 Schools](https://www.w3schools.com/css/default.asp) is a helpful resource for looking up other properties and values. You may also want to use refer to a[CSS cheatsheet, such as this one](https://courses.cs.washington.edu/courses/cse154/15sp/cheat-sheets/css-cheat-sheet.pdf).

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

## Font

**Font family** sets the font of a text. Because not all browsers support all fonts, it's a good idea to include the name of a specific font (such as 'Arial'), a 'fallback' font in case that font doesn't display, and the family the font belongs to ('sans-serif'). That way, a browser that doesn't support the font in question will substitute a similar one instead of the default.

```css
font-family: "Times New Roman", Times, serif;
```

If you want to get fancy, you can import web fonts from a repository such as [Google Fonts](https://fonts.google.com/).

## Position


**Text align** aligns an element to the left, center, or right.

```css
text-align: center;
```

Determining where elements appear on a page can get pretty complicated. CSS uses the **Box model** -- a box (really a series of boxes) that surrounds every element. Here are the main properties that control the size of those boxes.

**Padding** sets the space between an element's content and the border around it.

```css
padding: 10px;
padding-right: 10px
```

The **Border** is a line that surrounds the element -- it is invisible by default but will display if you set a size value. You can also set a color and a style.

```css
border: 15px solid green;
```

The **Margin** is the space between an element's border and whatever is around it, whether that's another element that contains it, the previous element, or the edge of the page.

```css
margin: 10px;
margin-top: 10px;
```

## Width and height

To specify a **width** or **height** for an element, use a value that is either a percentage of its container or a spatial metric (such as pixels):  

```css
width: 50%;
height: 40px;
```

## Other values

**Display** determines if an element is treated as an inline element or a 'block' on a new line. If you set display to `none`, an element will not be visible on the page.

```css
display: inline;
display: block;
display: none;
```

**List style** determines the type of marker or 'bullet' accompanies list items. To get rid of the markers, use `list-style-type: none;` 



[<<<Back](14-classes.md) | [Next>>>](16-creating_stylesheet.md)
