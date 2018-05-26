[<<<Back](filter.md) | [Next>>>](selectors.md)

# Classes and IDs

Classes and IDs can also assist with more fine-grained styling by allowing you to define your own selectors. The difference between classes and IDs is that IDs are unique, used to identify one specific element or part of an element, whereas classes are used to identify multiple instances of the same type of element.

Basically, if you're styling a part of your page that is unique, such as the navbar or footer, use an ID. If you're styling something that recurs in different places, like an info box or form field, use a class.

Incorporating classes and IDs into the styling of your document includes two steps:

- First, some CSS rules must be added to your stylesheet.
- Second, some HTML code that refers to the stylesheet must be added to your HTML document. Note that this is in addition to the general link to the stylesheet.

The code for classes and IDs is different in both CSS and HTML.

## Class selectors

Class selectors in CSS are denoted with a period in front of the class name you're creating. They look like this:

```css
.intro {
    font-family: arial;
    background-color: grey;
    color: dark grey;
}
```

...and in HTML they are incorporated into elements like this:

```html
<p class="intro">
  This is my introduction to my paragraph and I want to be distinguished from the rest of my content so I will add it as a class and note where the intros are found in my HTML.
</p>
```

## ID selectors 

Id slectors are denoted by a hash (`#`) (also known as a pound sign or octothorpe) before the ID name:

```css
#navbar {
    background-color: yellow;
    passing: 80px
}
```
...and in the HTML they are incorporated into elements like this:

```html
<ul id="navbar">
  <li> Home </li>
  <li> About </li>
</ul>
```

## Tip

If you run into an error, be sure to **check your syntax**. Often times it is a typo, or overlooking a semi-colon, etc. See the [Troubleshooting](troubleshooting.md) section for more information on common issues.

[<<<Back](filter.md) | [Next>>>](selectors.md)
