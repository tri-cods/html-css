[<<<Back](css_basic.md) | [Next>>>](rules.md)

# Integrating CSS and HTML

In order for CSS to inform the style of the content on the page, it must be integrated with your HTML. CSS can be integrated into your HTML in three ways: inline, internal, and external.

## Option 1: Inline

Inline styling adds CSS directly into the HTML of a page to adjust the style of particular parts of a page. 

For example, if you want your first paragraph to be red, but your second paragraph to be blue: 

```
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

```
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
    Heading 
    </h1>
	<p>
	Content of paragraph
	</p>
</body>
</html>
```

## Option 3: External

External styling creates a completely separate document for your CSS that will be linked to your HTML in the head section of your HTML document using the code below. This separate document is called a **stylesheet** and should be named `stlye.css`. This document must be stored in the same folder as the HTML document it is linked to.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>CSS Example</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
</body>
</html>
```

## Best Practices:
Option 3, external styling, is preferred by most web developers because it is considered best practice to keep your HTML and CSS separate. 

## ACTIVITY
Create a stylesheet through the command line. 

In your `index.html` document, link to your style sheet and re-save the file. 
<br/>
<br/>
## Command Line to create style sheet:
After opening terminal:
2. $ cd Desktop
3. $ cd Institute_Site
4. $ touch style.css
5. $ open style.css

## Where should the stylesheet be linked? 
The style sheet should follow `Option 3: External` - inserting the following code into the head element: 

`<link rel="stylesheet" href="style.css">`

[<<<Back](css_basic.md) | [Next>>>](rules.md)
