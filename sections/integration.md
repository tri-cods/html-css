[<<<Back](css_basic.md) | [Next>>>](rules.md)

# Integrating CSS and HTML

In order to CSS to inform the style of the content on the page, it must be integated with your HTML. CSS can be integrated into your HTML in three ways. 

## OPTION 1: Inline

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

## OPTION 2: Internal

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

External styling creates a completely separate document for your CSS that will be linked to your html in the head section of your html document using the code below. This separate document is called a **stylesheet** and should be named `stlye.css`. This document must be stored in the same file as the html document it is linked to.

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
Open up a new document in your Sublime Text editor. Save the document as `style.css` to the same folder as your HTML documents. In your `index.html` document, link to your style sheet and re-save the file. Be sure to add it in the correct place in the code. 
<br/>
<br/>

[<<<Back](css_basic.md) | [Next>>>](rules.md)