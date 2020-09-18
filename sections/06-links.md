← [Paragraphs and Headings](05-paragraphs-and-headings.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Images](07-images.md) →

---

# 6. Links

Links are the foundation of the World Wide Web, and thus are an important component of most websites. Hyperlinking text enables users to move between the different webpages on your site (sometimes in the form of a menu or navigation bar), or connect to other resources or information on other websites.

The `<a>` tag, or **anchor tag**, creates a link to another document. You can use the `<a>` tag to link to other documents or webpages you created for the same site or to documents located elsewhere on the web. You can also use it to link to a particular location on a page—we'll see an example of this in the section on Classes and IDs.

## Option One: Relative Links

Relative links take the current page as an origin point and search for other files within the same folder or directory. This method is useful for creating links to pages within your own site.

The following appears as a link to the `about.html` page in the same folder as `index.html`:

```html
<a href="about.html">About</a>
```

On your webpage it will appear as:

> [About](#)

This link is asking the browser to look for a file titled `about.html` in the same folder. If a file named `about.html` is not in the same folder, clicking the link will result in a `404` ("Page Not Found") error.

## Option Two: Absolute Links

An absolute link includes information that allows the browser to find resources on other websites. This information includes the site domain—such as `google.com`—and often the protocol—such as `http` or `https`.

```html
<a href="http://www.google.com">Google</a>
```

On your webpage it will appear as:

> [Google](http://www.google.com)

This pathway is directing your browser to look online for this text document at the URL address provided.

## More on links

Each example above includes an `href`—a hypertext reference—which is an example of an **attribute**. Attributes offer secondary information about an element.

The `<a>` tag, or anchor tag, creates a link. The text within the `<a>` and `</a>` tags, the anchor text, is what a visitor to the site will see and can click on. The `href=` attribute tells the browser where the user should be directed when they click the link.

There is another technical difference between the two options above.

## Relative vs. Absolute Links: When to use which

Use relative links when referring to pages on your own site. The main advantage of using relative links to pages on your site is that your site will not break if it is moved to a different folder or environment.

## Activity

1. Create a new text file called `about.html` in your `htmlpractice` folder. Copy over the HTML from your `index.html` file, but change the text in the `<h1>` element to "About."
2. In your `index.html` file, add a relative link leading to your "About" page.
3. Also add a relative link from your "About" page to your `index.html` page. In this link, call your `index.html` page "Home" (Reminder: `index.html` is the default homepage)
4. Lastly, include an absolute link to a page of your choosing. Remember that an absolute link includes the protocol (for example, `http:`) and also a domain (for example, `cuny.edu`), such as `http://cuny.edu/about`.
5. Re-save your text files and reopen or refresh them in your browser.

## Check if it worked

When your pages are updated, you should be able to navigate from your "Home" page to your "About" page, and vice versa. You should also be able to navigate to the external web page.

## Evaluation

Which of the following options is a relative link?
- `<a href="https://www.nytimes.com/">The New York Times</a>`
- `<a href="digitalProject.html">Digital Project</a>`*

## Keywords

Do you remember the glossary terms from this section?

- [Attributes](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/attribute.md)

---

← [Paragraphs and Headings](05-paragraphs-and-headings.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Images](07-images.md) →