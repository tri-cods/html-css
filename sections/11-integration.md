[<<<Back](10-css_basic.md) | [Next>>>](12-rules.md)

# Integrating CSS and HTML

In order for CSS to inform the style of the content on the page, it must be integrated with your HTML. CSS can be integrated into your HTML in three ways: inline, internal, and external.

## Option one: inline

Inline styling adds CSS directly into the HTML of a page to adjust the style of particular parts of a page.

For example, if you want the text of your first paragraph to be red, but the text of your second paragraph to be blue:

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>About</title>
    </head>

    <body>
        <p style="color: red">
            Content of paragraph
        </p>
        <p style="color: blue">
            Content of paragraph
        </p>
    </body>
</html>
```

## Option two: internal

Internal styling also adds CSS directly into the HTML, but keeps it separate from the content code of the page by adding it into the head using the `<style>` tag. When using internal styling you are providing styling rules for the entire page. For example, if you want all headings to be blue:

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>About</title>
        <style>
            h1 {
              color: blue;
            }
        </style>
    </head>

    <body>
        <h1>
            Heading One
        </h1>
        <p>
            Content of paragraph
        </p>
        <h1>
            Heading Two
        </h1>
        <p>
            Content of paragraph
        </p>
    </body>
</html>
```

## Option three: external (recommended)

External styling creates a completely separate document for your CSS that will be linked to your HTML in the head section of your HTML document using the code below. This separate document is called a **stylesheet** and should be named `style.css`. This document must be stored in the same folder as the HTML document it is linked to.

```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>CSS Example</title>
        <link rel="stylesheet" href="style.css" />
    </head>

    <body>
        ...
    </body>
</html>
```

## Best practices

It's best practice to use Option 3, external styling, for a number of reasons:

1. It helps us remember what each language focuses on: HTML is for _content_, CSS is for _styling_. (This is sometimes referred to as ["separation of concerns"](https://adamwathan.me/css-utility-classes-and-separation-of-concerns/))
2. It helps us maintain consistency across the various pages of our site; multiple HTML files can link to the same CSS file.
3. Because multiple HTML files can link to the same CSS file, it's not necessary to write the same CSS code multiple times. Once suffices.

Option 3, external styling, is preferred by most web developers because it's more manageable and because it lends itself to greater consistency across the entire site.

## Challenge

Create a stylesheet using the command line (following option 3, external styling, described above). In your `index.html` document, link to your style sheet and re-save the file.

If you need a reminder on which commands to use to create your new stylesheet file, see [here](_cli-reminder2.md).

To link your stylesheet with your `index.html` file, insert the following code into the head element of that `index.html` file:

```html
<link rel="stylesheet" href="style.css" />
```

[<<<Back](10-css_basic.md) | [Next>>>](12-rules.md)
