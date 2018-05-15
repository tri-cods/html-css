[<<<Back](filter.md) | [Next>>>](selectors.md)

# Classes and Ids

Classes and IDs can also assist with more fine-grained styling by allowing you to define your own selectors. The difference between classes and IDs is that **IDs are unique**, used to identify one specfic element or part of an element, whereas **classes are used to identify multiple instances of the same type of element**.

Incorporating classes and IDs into the styling of your document includes two steps: 

<ul>
	<li> First, some CSS rules must be added to your stylesheet; </li>
	<li> Second, some HTML code that refers to the stylesheet must be added to your HTML document. <i> Note that this is in addition to the general link to the stylesheet.</i> </li>
</ul>

**The code for classes and IDs is different in both CSS and HTML.**

## Class selectors
...look like this - the name of the selector preceeded by a full stop:

```
.intro {
	font-family: arial;
	background-color: grey;
	color: dark grey;
}
```

...and in HTML they are incorporated into elements like this:

```
<p class="intro">
		This is my introduction to my paragraph and I want to be distinguished from the rest of my content so I will add it as a class and note where the intros are found in my HTML.
</p>
```

## Id selectors 
...clook like this in the CSS - the name of the selector preceeded by a hashmark:

```
#navbar {
	background-color: yellow;
	passing: 80px
}
```

...and in the HTML they are incorporated into elements like this:

```
<ul id="navbar">
	<li> Home </li>
	<li> About </li>
</ul>
```

## Tip
If you run into an error, be sure to check your punctuation. Often times it is a mistype, or overlooking a semi-colon, etc.*

[<<<Back](filter.md) | [Next>>>](selectors.md)