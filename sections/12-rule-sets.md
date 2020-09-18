← [Integrating CSS and HTML](11-integrating-css-and-html.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Filtering](13-filtering.md) →

---

# 12. Rule Sets

CSS is based on selectors and declarations, which together form rule sets (or just "rules"). Rule sets comprise an external styling file with a `.css` extension. Here is the contents of a sample `.css` file:

```css
h1 {
    color: orange;
    font-style: italic;
}

p {
    font-family: sans-serif;
    font-style: normal;
}

#navbar {
    background-color: yellow;
    padding: 80px;
}

.intro {
    font-family: arial;
    background-color: grey;
    color: dark-grey;
}
```

The first rule (which starts with the `h1` selector) applies to all `<h1>` tags on each page where your HTML document links to your stylesheet, and changes the font style and display of those headings.

The lines within the curly braces (i.e. `{ ... }`) are called **declarations**, and they change the formatting of the elements in the HTML document. Each line in the declaration sets the value for a **property** and ends with a semicolon (`;`).

Note the different syntax being used to select items for for styling with rule sets. The bottom two selectors are used to apply rule sets to **IDs** and **classes**. In general, adding classes and IDs to HTML elements allows for more specific styling—more on these soon!

## Activity

Copy and paste the CSS rules above into your `style.css` file and re-save the file. Then open or refresh your `index.html` file in your browser and see what happens.

## What Should Happen?

The formatting of the text on your page should change accordingly. Your `<h1>` should be orange and italic, for example.

What are some other rules you might set for different HTML elements? Do a quick Google search for a CSS rule that changes the appearance of your page, such as putting a border around an element.

## Evaluation

How do we associate a CSS file with an HTML page?
- By including a link to the CSS file in the HTML page's `<head>` element.*
- By putting the CSS file in the same folder as the HTML page.

## Keywords

Do you remember the glossary terms from this section?

- [CSS Selectors](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/cssselectors.md)
- [Class](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/class.md)
- [ID](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/id.md)

---

← [Integrating CSS and HTML](11-integrating-css-and-html.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Filtering](13-filtering.md) →