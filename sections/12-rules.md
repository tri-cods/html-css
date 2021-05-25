[<<<Back](11-integration.md) | [Next>>>](13-filter.md)

# Rule Sets

A CSS document is comprised of rule sets that define individual display properties. For example: 

```css
h1 {
    color: orange;
}
```

Each rule set includes:
- A **selector** (here, `h1`) which identifies the HTML elements to which the rule will apply (i.e., all `<h1>` elements in your document)
- A set of curly braces (i.e. `{ }`) 
- Within the braces, one or more **declarations** (`color: orange;`) that tells the browser how to format or style those elements
- These consist of a display **property** (`color`) followed by a colon `:`, at least one **value** (`orange`) and then a semicolon `;`

Unlike an HTML document, a CSS document doesn't need a specific overall structure, but it does require specific formatting: 

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

Note the different syntax being used to select items for for styling with rule sets. The bottom two selectors are used to apply rule sets to elements with a particular **id** or **class** attribute. In general, adding classes and ids to HTML elements allows for more specific styling — more on these soon!

## Challenge

Copy and paste the CSS above into your `style.css` file and re-save the file. Then open or refresh your `index.html` file in your browser and see what happens.

## What should happen?

The formatting of the text on your page should change accordingly. Your `<h1>` should be orange and italic, for example.

What are some other rules you might set for different HTML elements? Do a quick Google search for a CSS rule that changes the appearance of your page, such as putting a border around an element.

[<<<Back](11-integration.md) | [Next>>>](13-filter.md)
