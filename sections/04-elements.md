[<<<Back](03-basic.md) | [Next>>>](05-p_and_h.md)

# Tags and Elements

Tags and elements are the structuring components of html webpages.

**Elements** identify the different parts of a page, such as paragraphs, headings, titles, body text, images and more. Elements are demarcated by tags which enclose the content of an element (ex. `<head>` and `</head>` are tags that denote the head element of your page).

**Tags** demarcate elements in one of two ways. As with the paragraph element below, an element can have an opening and a closing tag, with content in between.

```html
<p>This is a paragraph.</p>

<p>
    This is also a paragraph.
</p>
```

Elements which have an opening and closing tag can have other elements inside them. Inside the paragraph element below is a strong element, which emphasizes the included text by making it bold.

```html
<p>
    When I came home from school, I saw he had <strong>stolen</strong> my chocolate pudding.
</p>
```

Some elements, such as the image element, have self-closing tags or **void tags**. Because these elements do not contain displayed text or other nested elements, they only need a single tag `<img/>` rather than a tag to open `<p>` and a tag to close `</p>`

```html
<img alt="This is an image" src="image.jpeg" />
```

You'll notice that the `img` element above does have additional information within the tag itself: these are called **attributes**. Attributes offer secondary information about an element or modify its functionality. In this case, the `img` has a `src` or source attribute, which tells the browser where to find the image file to display, and an `alt` attribute, which provides an alternative text description of the image content and is crucial for web accessibility. We will discuss both attributes in more detail in the [images section](07-images.md).   

If you look back at the basic template in your `index.html` file, you'll see that the main sections of your file have opening and closing tags. Each of these main elements will eventually enclose several nested elements to structure the content of our website.

[<<<Back](03-basic.md) | [Next>>>](05-p_and_h.md)
