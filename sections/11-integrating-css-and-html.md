← [CSS Basics](10-css-basics.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Rule Sets](12-rule-sets.md) →

---

# 11. Integrating CSS and HTML

In order for CSS to inform the style of the content on the page, it must be integrated with your HTML. CSS can be integrated into your HTML in three ways:

1. inline
2. internal
3. external (_recommended_)

## Option 1: Inline

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

## Option 2: Internal

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

## Option 3: External (Recommended)

External styling creates a completely separate document for your CSS that will be linked to your HTML in the head section of your HTML document using the code below. This separate document is called a _stylesheet_ and is often named `style.css`. The document is linked through a void `<link>` tag that lives inside the parent `<head>` tag. Its `href` attribute is a relative link to the document somewhere in relation to the document that references it.

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

## Best Practices

It's best practice to use Option 3, external styling, for a number of reasons:

1. It helps us remember what each language focuses on: HTML is for _content_, CSS is for _styling_. (This is sometimes referred to as the principle of ["separation of concerns"](https://adamwathan.me/css-utility-classes-and-separation-of-concerns/))
2. It helps us maintain consistency across the various pages of our site as _multiple HTML files can link to the same stylesheet_.
3. Because multiple HTML files can link to the same CSS file, it's not necessary to write the same CSS code multiple times. Once suffices. (This is sometimes referred to as the ["Don't Repeat Yourself" principle](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself), or simply _DRY_.)

Option 3, external styling, is preferred by most web developers because it's more manageable and because it lends itself to greater consistency across the entire site.

## Activity

Create a blank stylesheet using the command line (following option 3, external styling, described above). In your `index.html` document, link to your style sheet and re-save the file.

To link your stylesheet with your `index.html` file, insert the following code into the head element of that `index.html` file:

```html
<link rel="stylesheet" href="style.css" />
```

## Evaluation

Is the following code-snippet an example of inline styling or internal styling?
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>Homepage</title>
        <style>
            h1 {
              font-family: monospace;
            }
            p {
             font-family: fantasy;
            }
        </style>
    </head>

    <body>
        <h1>
            Online Library for All!
        </h1>
        <p>
            Free books here!
        </p>
    </body>
</html>
```
- Inline Styling
- Internal Styling*

---

← [CSS Basics](10-css-basics.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Rule Sets](12-rule-sets.md) →