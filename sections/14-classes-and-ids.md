← [Filtering](13-filtering.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Useful Properties](15-useful-properties.md) →

---

# 14. Classes and IDs

Classes and IDs enable more fine-grained styling by allowing you to define your own selectors. The difference between classes and IDs is that IDs are unique, used to identify one specific element or part of an element, whereas classes are used to identify multiple instances of the same type of element.

Basically, if you're styling a part of your page that is unique, such as the navbar or footer, use an ID. If you're styling something that recurs in different places, like an info box or form field, use a class.

Incorporating classes and IDs into the styling of your document includes two steps:

1. Some HTML code that CSS selectors can refer back to must be added to your HTML document.
2. CSS rules that select that code must be added to your style sheet.

The code for classes and IDs is different in both CSS and HTML.

## HTML Code

In HTML, classes and ids are added to the first part of a tag. Here's an example of what HTML code with classes and ids looks like:

```html
<ul id="navbar">
    <li>Home</li>
    <li>About</li>
</ul>


<h1 class="football">Football teams</h1>

<ul>
    <li class="football" id="colts">Indianapolis Colts</li>
    <li class="football" id="packers">Green Bay Packers</li>
</ul>


<h1 class="baseball">Baseball teams</h1>

<p>American League teams</p>
<ul>
    <li class="baseball american" id="twins">Minnesota Twins</li>
    <li class="baseball american" id="tigers">Detroit Tigers</li>
</ul>

<p>National League teams</p>
<ul>
    <li class="baseball national" id="dodgers">Los Angeles Dodgers</li>
    <li class="baseball national" id="mets">New York Mets</li>
</ul>
```

Note that it's possible to assign more than one class to an element—just leave a blank space between the two classes, as in the baseball examples above.

Bonus: ID selectors can be used to create links that can be used for navigation _within_ a page. For example, to add a link to the page that takes the user directly to the line that reads "New York Mets," we might write a HTML link like this: `<a href="#mets">Mets</a>`.

## CSS Selectors

Class selectors in CSS are denoted with a period in front of the class name you're creating. They look like this:

```css
#navbar {
    padding: 80px;
    background-color: red;
    color: white;
}

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

## ID Selectors

...look like this in the CSS—the name of the selector preceeded by a hashmark (`#`) (also known as a pound sign or octothorpe):

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

_If you run into an error, be sure to check your punctuation. Oftentimes the problem is a typo, or overlooking a semi-colon, a period, etc._ See the [Troubleshooting](https://curriculum.dhinstitutes.org/workshops/html-css/lessons/?page=17) section for more information on common issues.

## Evaluation

True or False: Classes are used to create categories of related elements, IDs are used create unique identifiers.
- True*
- False

## Keywords

Do you remember the glossary terms from this section?

- [CSS Selectors](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/cssselectors.md)
- [Class](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/class.md)
- [ID](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/id.md)

---

← [Filtering](13-filtering.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Useful Properties](15-useful-properties.md) →