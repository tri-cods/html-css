[<<<Back](integration.md) | [Next>>>](filter.md)

# Rule Sets

CSS is based on selectors and declarations, which together form rule sets (or just "rules"). Rule sets (included in a .css file) look like this:

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

The lines within the curly braces (i.e. `{ }`) are called **declarations**, and they change the formatting of the elements in the HTML document. Each declaration ends in a semicolon (`;`).

Note the different syntax being used to select items for for styling with rule sets. The bottom two selectors are used to apply rule sets to **ids** and **classes**. In general, adding classes and ids to HTML elements allows for more specific styling — more on these soon!

## Challenge

Copy and paste the CSS above into your `style.css` file and re-save the file. Then open or refresh your `index.html` file in your browser and see what happens.  

## What should happen? 

The formatting of the text on your page should change accordingly. Your `<h1>` should be orange and italic, for example.

What are some other rules you might set for different HTML elements? Do a quick Google search for a CSS rule that changes the appearance of your page, such as putting a border around an element.

[<<<Back](integration.md) | [Next>>>](filter.md)
