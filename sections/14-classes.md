[<<<Back](13-filter.md) | [Next>>>](15-properties.md)

# Classes and IDs

Classes and IDs enable more fine-grained styling by allowing you to define your own selectors. The difference between classes and IDs is that IDs are unique, used to identify one specific element or part of an element, whereas classes are used to identify multiple instances of the same type of element.

Basically, if you're styling a part of your page that is unique, such as the navbar or footer, use an ID. If you're styling something that recurs in different places, like an info box or form field, use a class.

Incorporating classes and IDs into the styling of your document includes two steps:

1. Some HTML code that CSS selectors can refer back to must be added to your HTML document.
2. CSS rules that select that code must be added to your style sheet.

The code for classes and IDs is different in both CSS and HTML.

## HTML code

In HTML, classes and IDs are added to the first part of a tag as attributes: `id="id-name"` and `class="class-name"`. For example:

```html
<ul id="navbar">
    <li>Home</li>
    <li>About</li>
</ul>

<h1>Teams</h1>

<h2 class="football">Football teams</h2>
<ul>
    <li class="football" id="colts">Indianapolis Colts</li>
    <li class="football" id="packers">Green Bay Packers</li>
</ul>


<h2 class="baseball">Baseball teams</h2>

<h3>American League teams</h3>
<ul>
    <li class="baseball american" id="twins">Minnesota Twins</li>
    <li class="baseball american" id="tigers">Detroit Tigers</li>
</ul>

<h3>National League teams</h3>
<ul>
    <li class="baseball national" id="dodgers">Los Angeles Dodgers</li>
    <li class="baseball national" id="mets">New York Mets</li>
</ul>
```

Note that it's possible to assign more than one class to an element — just leave a blank space between the two classes, as in the baseball examples above.

Bonus: ID selectors can also be used to create links that can be used for navigation *within* a page. For example, to add a link to the page that takes the user directly to the line that reads "New York Mets," we might write HTML like this: `<a href="#mets">Mets</a>`.

## CSS selectors

Class selectors in CSS are denoted with a period in front of the class name you're creating: `.class-name`. For example:

```css

.football {
  font-family: arial;
  background-color: lightgrey;
  color: blue;
}

.baseball {
  font-weight: bold;
  color: green;
}

.american {
  background-color: yellow;
}
```
...and in the HTML they are incorporated into elements like this:

```html

<h2 class="football">Football teams</h2>

```

## ID selectors

...look like this in the CSS—the name of the selector preceeded by a hashmark (`#id-name`) (also known as a pound sign or octothorpe):

```css
#navbar {
    background-color: yellow;
    padding: 80px;
}
```

...and in the HTML they are incorporated into elements like this:

```html
<ul id="navbar">
    <li>Home</li>
    <li>About</li>
</ul>
```

## Tip

*If you run into an error, be sure to check your punctuation. Oftentimes the problem is a typo, or overlooking a semi-colon, a period, etc.* See the [Troubleshooting](17-troubleshooting.md) section for more information on common issues.

[<<<Back](13-filter.md) | [Next>>>](15-properties.md)
