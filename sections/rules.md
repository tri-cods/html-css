[<<<Back](integration.md) | [Next>>>](filter.md)

# Rule Sets

CSS is based on rules. Rule sets—that are included in a .css file—look like this:

```css
h1 {
    color: orange;
    font-style: italic;
}
p {
    font-family: san serif;
    font-style: normal;
}
#navbar {
    background-color: yellow;
    padding: 80px;
}
.intro {
    font-family: arial;
    background-color: grey;
    color: dark grey;
}
```

The first rule applies to all `<h1>` tags on each page where your HTML document links to your stylesheet, and changes the font style and display of those headings.

The lines within the curly braces (i.e. `{ }`) are called **selectors**, and they change the formatting of the elements in the HTML document. Each selector ends in a semicolon (`;`).

Note the different syntax being used for the different rule sets. The bottom two are specific kinds of rule sets called **classes** and **ids**. In general, classes and ids allow for more specific styling—more on these soon! 

## Challenge

Copy and paste the CSS above into your `style.css` file and re-save the file. Then open or refresh your `index.html` file in your browser and see what happens.  

## What should happen? 

The formatting of the text on your page should change accordingly. Your `<h1>` should be orange and italic, for example.

What are some other selectors you might set for different HTML elements? Do a quick Google search for a CSS element that changes the appearance of your page, such as putting a border around an element.

[<<<Back](integration.md) | [Next>>>](filter.md)
