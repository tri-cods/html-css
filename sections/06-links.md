[<<<Back](05-p_and_h.md) | [Next>>>](07-images.md)

# Links

Links are the foundation of the World Wide Web, and thus are an important component of most websites. Hyperlinking text enables users to move between the different webpages on your site (sometimes in the form of a menu or navigation bar), or connect to other resources or information on other websites.

The `<a>` tag, or **anchor tag**, creates a link to another document. You can use the `<a>` tag to link to other documents or webpages you created for the same site or to documents located elsewhere on the web. (You can also use it to link to a particular location on a page—we'll see an example of this in the section on classes and ids.) 

```html
<a href="https://en.wikipedia.org">Wikipedia</a>
```

The text between the `<a>` and `</a>` tags, the **anchor text**, is what a visitor to the site will see and can click on. You'll notice that the `<a>` tag above includes a url preceded by `href=`: this tag, short for hypertext reference, tells the browser where the user should be directed when they click the link. The `href` is an example of an element **attribute**. Attributes appear within the opening element tag and offer secondary information about an element. 

## Relative vs. Absolute Links

A **relative link** takes the current document as an origin point and search for other files within the same folder or directory. This method is useful for creating links to pages within your own site.

The following appears as a link to the `about.html` page in the same folder as `index.html`:

```html
<a href="about.html">About</a>
```

On your webpage it will appear as:

> [About](#)

This link is asking the browser to look for a file titled `about.html` in the same folder. If a file named `about.html` is not in the same folder, clicking the link will result in a `404` ("Page Not Found") error.

An **absolute link** resembles a typical URL, and allows the browser to find resources on other websites. This information includes the site domain—such as `wikipedia.org`—and often the protocol—such as `http` or `https`.

```html
<a href="https://en.wikipedia.org">Wikipedia</a>
```

On your webpage it will appear as:

> [Wikipedia](https://en.wikipedia.org)

This pathway is directing your browser to look online for this text document at the URL address provided.

Use relative links when referring to pages on your own site. That way your site will not break if it is moved to a different folder or environment.

## Activity

1. Create a new text file called `about.html` in your `htmlpractice` folder. Copy over the HTML from your `index.html` file, but change the text in the `<h1>` element to "About."
2. In your `index.html` file, add a relative link leading to your About page.
3. Also add a relative link from your `About page` to your `index.html` page. In this link, call your `index.html` page `Home` (Reminder: `index.html` is the default homepage)
4. Lastly, include an absolute link to a page of your choosing. Remember that an absolute link includes the protocol (for example, `http:`) and also a domain (for example, `cuny.edu`), such as `http://cuny.edu/about`.
5. Re-save your text files and reopen or refresh them in your browser.

## Check if it worked

When your pages are updated, you should be able to navigate from your Home page to your About page, and vice versa. You should also be able to navigate to the external web page.

[<<<Back](05-p_and_h.md) | [Next>>>](07-images.md)
