# Introduction

Websites seem like these magical things that appear when we open our web browser (i.e. Chrome, Firefox, Safari). We know that websites are hypertext, meaning that we can click between links, travelling from page to page until we find what we need. What may be less obvious about websites is that, fundamentally **websites are plain text documents**, usually written in HTML or another web-based markup language, such as XML or XHTML.

*Fun fact*: **More than 90% of all websites (whose markup language we know) use HTML**
[(w3techs.com)](https://w3techs.com/technologies/details/ml-html/all/all).

## Hypertext Markup Language (HTML)

HTML is a markup language used to write web-based documents. It enables us to provide web browsers with information about the _content_ of a document. We can, for example, indicate that some part of our document is a paragraph, image, heading, or link. The browser uses this information when displaying the document for users.

## Markup language vs. programming Language

HTML is a *markup* language, not a programming language. Programming languages are used to transform data, by creating scripts that organize an output of data based on a particular input of data. A markup language is used to control the presentation of data.

For a practical example of this difference, we can think about tables. A programming language can help you search through a table, understand the kinds of data the table includes, find particular data points, or transform its content into other kinds of data, such as frequencies. A markup language would instead determine the content, layout, and visual presentation of the table.

Fundamentally, then, a script or program is a set of instructions given to the computer. A document in a markup language determines how information is presented to a user.

**NOTE - Markup vs Markdown:** Markdown and HTML are both types of markup languages; Markdown is a play on words. Markup languages help format content.

## Cascading Style Sheets (CSS)

CSS is usually used in conjunction with HTML. HTML tells the browser what the different parts of a document _are_. CSS tells the browser what the parts of the document should _look like_. It is essentially a set of rules that are applied when rendering an HTML document. Its name—Cascading Style Sheets—refers to the fact that there is an order of precedence in how the browswer applies CSS rules to a document. More specific rules overwrite less specific rules.

## Where does the internet come in?

Together, these languages can be used to write and style a website using a text editor (such as VS Code) directly from your computer. No internet access needed.

However, internet access is necessary if you plan on making your website available to the public. At the end of this workshop, we will briefly discuss [how to get your website from your local computer onto the internet](19-public.md).

# Opening Activity

1. Open a web browser. (NOTE: please use Firefox or Chrome. Safari will not allow you to complete this activity.)
2. Go to any webpage.
3. Open the secondary menu (using a mouse, this would be the menu that opens when you right click on the page; on Mac computers, this is usually a two-finger tap on the track pad, or you can press the "control" button then click the track pad).
4. Select ‘View Page Source’ from the dropdown menu.

![Image showing dropdown menu that appears when right clicking on a website in Chrome or Firefox](images/page_source.jpeg)

## What you're seeing

A second tab should open in your browser displaying the underlying code of the page. This is the code that is used to make and render the page in your web browser.

![Image showing the page source information and underlying HTML code of a webpage](images/pageSource.PNG)

In this session, we are going to learn how to read and write this code, and render it in the browser on your local computer. At the end we will discuss the next steps for how you could host your new website, making it available for browsing by others via the internet.

# Basic Template for HTML

Below is a basic template for an empty HTML Document.

```html
<!DOCTYPE html>
<html lang="en">

  <head>
      ...
  </head>

  <body>
      ...
  </body>

</html>
```

HTML documents start with a `DOCTYPE` declaration that states what version of HTML is being used. This tells the browser how to read the code below it to render the page. If the webpage were written with a different markup language (i.e. XML, XHTML), it would tell you here.

After the `DOCTYPE`, we see the start of the **Root Element**. EVERYTHING—all content—that you want presented on this page and all information about how you want that information to be organized and styled goes in the root element, and it is demarcated by `<html>` and `</html>`.

The root element begins by indicating which language the document is written in; and in this basic template, `en` tells us and the computer that we are writing in English.

Within the root element of the basic template above, you'll notice the two main sections of all HTML documents: a head section (demarcated by `<head>` and `</head>`) and a body section (demarcated by `<body>` and `</body>`).

The **head section** contains basic information about the file such as the title, keywords, authors, a short description, and so on. This is also where you will link to your CSS stylesheet which describes how you want the page styled—colors, fonts, size of text, and positioning of elements on the page.

The **body section** contains the content of the page, including paragraphs, images, links, and more, and indicates how this content is to be structured on the page.

## Activity

Create a folder called `htmlpractice` in your projects folder (`~/Desktop/projects/htmlpractice`). If you haven't created a projects folder in an earlier session, you can create one now. Inside that folder, create a new text file and save it as `index.html`.

Let's use the command line to create the new folder and file:

1. Open your terminal.
2. Navigate to your projects folder using this command:

    ```sh
    $ cd ~/Desktop/projects
    ```

3. Create a new folder:

    ```sh
    $ mkdir htmlpractice
    ```

4. Use your VS Code text editor to create a file called `index.html`: `code index.html`.
5. Paste the template above (starting with `<!DOCTYPE html>`) into the new file.

The `index.html` file is your default homepage for the website we are creating. This is an industry standard, because web browsers tend to recognize the `index.html` page as the opening page to the directory that is your website. See [here](https://www.lifewire.com/index-html-page-3466505) for more explanation.

Once you've created your new file, open it with a web browser using your graphical user interface:

On macOS, click on the Finder in your dock (the apps at the bottom of the screen) and click on Desktop on the left. From there, navigate to `projects`, then `htmlpractice`. Alternately, you can click the projects folder icon on your Desktop and find it from there. If you're using a Mac and would prefer to use the command line, you can also type `open index.html` from within your `htmlpractice` folder.

On Windows, click the `projects` folder icon on your desktop. Navigate to `projects`, then `htmlpractice`. Double click the `index.html` file. If it does not open in a browser, right click the `index.html` icon and select "Open with..." from the menu. Select Firefox or Google Chrome from the app list that appears.

### What happens?

When you open the empty template, you'll see only a blank web page. Open your secondary menu (right click on Windows, hold control and click with macOS) and view the page source. How can you explain what happens when you open these text files?

## What should happen when I open each of my two new files?

When you "View Page Source," you should see the code for the basic template.

No content renders on the page, because there is no content in the template at this time.

# Tags and Elements

Tags and elements are the structuring components of html webpages.

**Elements** identify the different parts of a page, such as paragraphs, headings, titles, body text, images and more. Elements are demarcated by tags which enclose the content of an element (ex. `<head>` and `</head>` are tags that denote the head element of your page).

**Tags** demarcate elements in one of two ways. As with the paragraph element below, an element can have an opening and a closing tag, with the content in between.

```html
<p>This is a paragraph.</p>

<p>
    This is also a paragraph.
</p>
```

Elements which have an opening and closing tag can have other elements inside them. Inside the paragraph element below is a `strong` element, which emphasizes the included text by making it bold.

```html
<p>
    When I came home from school, I saw he had <strong>stolen</strong> my chocolate pudding.
</p>
```

Other elements have self-closing tags as with the `img` (image) element below. These tags are also called **void tags**.

```html
<img src="image.jpeg" />
```

These elements don't require a separate closing tag. Closing tags aren't needed because you wouldn't add content inside these elements. For example, it doesn't make sense to add any additional content inside an image.

Below is HTML that adds alternative text to an image—or text that describes the image. This information added is an attribute—or something that modifies the default functionality of an element.

```html
<img alt="This is an image" src="image.jpeg" />
```

Adding alternative text to an image, as was done in this example, is vitally important. That information makes the image more accessible to those viewing your site. For instance, users with poor vision who may not be able to see your image will still understand what it is and why it's there if you provide alternative text describing it.

If you look back at the basic template in your `index.html` file, you'll see that the main sections of your file have opening and closing tags. Each of these main elements will eventually hold many other elements, many of which will be the content of our website.

# Paragraphs and Headings

Paragraphs and headings are the main textual elements of the body of your webpages. Because these contain content that you want to organize and display on your webpage, these are entered in the body element.

The `<h1>`, `<h2>`, `<h3>`, etc. tags denote **headings** and **subheadings**, with `<h1>` being the largest and `<h6>` the smallest.

The `<p>` tags denote **paragraphs**, or blocks of text.

```html
<!DOCTYPE html>
    <html lang="en">

    <head>
        <title>A boring story</title>
    </head>

    <body>
        <h1>
            Cleaning my boiler
        </h1>
        <p>
            When I got to my basement that day, I knew that I just had to clean my boiler. It was just too dirty. Honestly, it was getting to be a hazard. So I got my wire brush and put on my most durable pair of boiler-cleaning overalls. It was going to be a long day.
        </p>
    </body>

</html>
```

Note that the `<title>` is in the `<head>` element, which is where information about the webpage goes. The title doesn't appear on the page, but instead elsewhere in the browser when the page is displayed. For example, in Chrome, the title appears on the tab above the navbar.

![Image showing where the title appears in the Chrome web browser](images/title.png)

Note also that the elements and tags used in HTML have _meaning_. They provide information about the structure of a web page, showing how its parts work together. Those who make use of assistive technologies such as screen readers rely on this semantic information to navigate the page. Thus, it's important to use elements such as headers only when the information being marked calls for it. Making text large and/or bold for visual effect should be done using CSS. The Mozilla Developer Network has some good [introductory information on semantic HTML](https://developer.mozilla.org/en-US/docs/Glossary/Semantics#Semantics_in_HTML).

## Activity

Using your text editor, add the following to your `index.html`:

- Title
- Heading
- Paragraph

Then, re-save the file. Open it in your browser again or refresh the page if still opened.

What do you notice about how the information is organized in the webpage? In other words, where are the title, heading, and paragraph text?

## What should you see?

The heading should appear at the top of the page, followed by the paragraph text. The heading text should be larger. The title should appear in the browser window tab.

![Image of the boiler example above rendered in Google Chrome](images/boiler-example.png)

# Links

Links are the foundation of the World Wide Web, and thus are an important component of most websites. Hyperlinking text enables users to move between the different webpages on your site (sometimes in the form of a menu or navigation bar), or connect to other resources or information on other websites.

The `<a>` tag, or **anchor tag**, creates a link to another document. You can use the `<a>` tag to link to other documents or webpages you created for the same site or to documents located elsewhere on the web. You can also use it to link to a particular location on a page—we'll see an example of this in the section on classes and ids.

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

Each example above includes an `href` tag. The `href` tag, short for hypertext reference, is an example of an **attribute**. Attributes offer secondary information about an element.

The `<a>` tag, or anchor tag, creates a link. The text within the `<a>` and `</a>` tags, the anchor text, is what a visitor to the site will see and can click on. The `href=` attribute tells the browser where the user should be directed when they click the link.

There is another technical difference between the two options above.

## Relative vs. Absolute Links: When to use which

Use relative links when referring to pages on your own site. The main advantage of using relative links to pages on your site is that your site will not break if it is moved to a different folder or environment.

## Activity

1. Create a new text file called `about.html` in your `htmlpractice` folder. Copy over the HTML from your `index.html` file, but change the text in the `<h1>` element to "About."
2. In your `index.html` file, add a relative link leading to your About page.
3. Also add a relative link from your `About page` to your `index.html` page. In this link, call your `index.html` page `Home` (Reminder: `index.html` is the default homepage)
4. Lastly, include an absolute link to a page of your choosing. Remember that an absolute link includes the protocol (for example, `http:`) and also a domain (for example, `cuny.edu`), such as `http://cuny.edu/about`.
5. Re-save your text files and reopen or refresh them in your browser.

## Check if it worked

When your pages are updated, you should be able to navigate from your Home page to your About page, and vice versa. You should also be able to navigate to the external web page.

# Images

Images are another important component of websites. Sometimes these just help bring your website to life, but other times they can help communicate information to users.

Images are created with the `<img>` tag. Similar to the `<a>` tag, `<img>` requires an attribute, in this case `src`. The `src` attribute stands for "source" and communicates secondary information to your browser that identifies and locates the image. Unlike many other tags, the `<img>` tag does not need to be closed, making it an example of a void tag.

The following element pulls in an image located in the same folder as the `.html` file:

```html
<img src="scream.jpeg" />
```

The same rules apply here as with the `href` attribute: if the image is not located in the same folder as the document you are writing in, the browser won't find it. If the browser cannot find an image resource, you will see a broken image icon, such as this one from Chrome:

![Chrome broken image icon](images/broken.png)

Note: Some sites use a lot of images. When this is the case, it can be helpful to keep images in a separate folder within your site's structure. To enable the browser to find an image in that case, just add the directory in front of the file name. For example, if you have a folder named images in the same folder as your index.html file, and scream.jpeg is in that folder, you'd change the void tag above to `<img src="/images/scream.jpeg" />`.

## Making images accessible

As briefly noted earlier, alternative text, or alt text, is descriptive "text associated with an image that serves the same purpose and conveys the same essential information as the image" (see [Wikipedia Manual of Style/Accessibility/Alternative Text for Images](https://en.wikipedia.org/wiki/Wikipedia:Manual_of_Style/Accessibility/Alternative_text_for_images) for more), and is important for ensuring content conveyed by images is accessible to all.

To add alternative text to an image, you add an additional attribute, `alt` followed by your descriptive text. For example:

```html
<img src="filename.png" alt="Text in these quotes describes the image" />
```

For more information, see what the [Social Security Administration](https://www.ssa.gov/accessibility/files/SSA_Alternative_Text_Guide.pdf) has to say.

## What images can I use on my site?

If you're planning to use images that you did not take or make yourself, you'll need to use "public domain" or "open license" images.

This [guide by the OpenLab at City Tech](https://openlab.citytech.cuny.edu/blog/help/following-copyright-guidelines-for-images/) includes more information on licensure and a list of places where you can find reuseable images.

## Activity

Download and save an image from the web, or move an image from your computer into the same folder as your `index.html` file.

Tip: Give the file a simple name. Also, the name **cannot** have spaces. A good practice is to use either dashes or underscores where there would otherwise be spaces. For example: `this-is-an-image.jpg` or `this_is_an_image.jpg`.

Using the code above as a reference, add that image into your `index.html` file, re-save the file, and re-open or refresh the page in your browser. Your image should now appear on the page.

# Conventions

As we’ve gone through the different components of creating a webpage, you likely have noticed some common conventions or industry standards for creating a webpage using HTML. Can you guess any of these?

Here are a few examples:

- Some tags are self-closing, while others require a closing tag. Self-closing tags are called void tags, and are generally self-closing because you wouldn't need or want to add another element within a tag. They also generally end with a backslash (`/`) to mark the end of the tag.
- Use lower case. While HTML is not case sensitive, it makes scanning the code easier, and makes it look more consistent.
- Your code should be nested. This is not a technical necessity either — blank space has no meaning in html. However, this makes it easier to scan the code quickly, which is particularly helpful when you run into errors!

# Challenge: Create an Institute Website

For this challenge, practice using the command line. If you need a reminder of which commands to use to create new folders and files, see [here](_cli-reminder.md).

Using the tags we've just reviewed, and two additional ones (see below) begin creating an introductory page for your future Digital Humanities Institute.


In your `projects` folder on your desktop, create a new folder called `website`. Create a `index.html` file inside that folder. This will be the homepage or landing page of your site.

Add HTML to your `index.html` file. This page should include the following:

- Doctype
- Root element
- Head and a body
- Title for the page
- One heading
- One paragraph
- One image with alt text
- A menu or navigation bar that links to your Home and About pages

Think about the order of your content as you assemble the body of your page.

Don't worry about getting the content just right, as much as using this exercise to review the structure of a webpage, and practice creating a webpage.

## Additional Tags

Here are two additional tags that might come in handy in assembling your page:

To make a list, you open and close it with the `ul` tags, and each item is an enclosed `li` tag:

```html
<ul>
    <li> item 1 </li>
    <li> item 2 </li>
    <li> item 3 </li>
</ul>
```

The HTML above will produce an unordered (bulleted) list. To create an ordered (numbered) list instead, just substitute `<ol>` and `</ol>` for `<ul>` and `</ul>`.

(This may come in handy when making your menu or navigation bar.)

To make a line break or give space between different elements:

```html
<br />
```

## Further challenge

Add a table containing a schedule of events to your Institute website. You can learn more about making tables using HTML [here](https://www.w3schools.com/html/html_tables.asp).

# CSS Basics

CSS stands for Cascading Style Sheets. This language works in coordination with HTML, but is its own language with its own rules and terminology. In contrast to HTML, which is responsible for the content of the page, CSS is responsible for the presentation of the page.

Examples of what CSS can help you determine include:

- What background color you want to use for the page or a paragraph.
- What font or font size you want for your headings or your normal text.
- How large you want the images, and whether you want them aligned center, left, or right.
- Where elements appear on the page.
- Whether elements are visible to a user or not.

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

# Rule Sets

CSS is based on selectors and declarations, which together form rule sets (or just "rules"). Rule sets (included in a .css file) look like this:

```css
h1 {
    color: orange;
    font-style: italic;
}

p {
    font-family: sans-serif;
    font-style: normal;
}

#navbar {
    background-color: yellow;
    padding: 80px;
}

.intro {
    font-family: arial;
    background-color: grey;
    color: dark-grey;
}
```

The first rule (which starts with the `h1` selector) applies to all `<h1>` tags on each page where your HTML document links to your stylesheet, and changes the font style and display of those headings.

The lines within the curly braces (i.e. `{ }`) are called **declarations**, and they change the formatting of the elements in the HTML document. Each line in the declaration sets the value for a **property** and ends with a semicolon (`;`).

Note the different syntax being used to select items for for styling with rule sets. The bottom two selectors are used to apply rule sets to **ids** and **classes**. In general, adding classes and ids to HTML elements allows for more specific styling — more on these soon!

## Challenge

Copy and paste the CSS above into your `style.css` file and re-save the file. Then open or refresh your `index.html` file in your browser and see what happens.

## What should happen?

The formatting of the text on your page should change accordingly. Your `<h1>` should be orange and italic, for example.

What are some other rules you might set for different HTML elements? Do a quick Google search for a CSS rule that changes the appearance of your page, such as putting a border around an element.

# Filtering

Some of you may be wondering whether it matters what order you add the rule sets to your `style.css` document. The answer is no. CSS has an automatic filtering function where **the most specific rule in CSS always takes precedence.**

So if your stylesheet contained the following rule sets:

```css
p {
    color: green;
}

p strong {
    color: red;
}
```

...then the text of your paragraph would be green, but where the strong tag is found in the paragraph, the text would be bold and red. In other words, the more specific styling for the `<strong>` text in your paragraph will override the less specific styling of the paragraph in general. This would occur **regardless of the order these rule sets appear in the stylesheet.**

This rule also applies to how you integrate CSS into your HTML to style your content. For example, if you link to an external stylesheet, and you add inline or internal CSS into your HTML, the inline or internal CSS will override the rules set in the external stylesheet. Similarly, the inline CSS will override the internal CSS.

# Classes and IDs

Classes and IDs enable more fine-grained styling by allowing you to define your own selectors. The difference between classes and IDs is that IDs are unique, used to identify one specific element or part of an element, whereas classes are used to identify multiple instances of the same type of element.

Basically, if you're styling a part of your page that is unique, such as the navbar or footer, use an ID. If you're styling something that recurs in different places, like an info box or form field, use a class.

Incorporating classes and IDs into the styling of your document includes two steps:

1. Some HTML code that CSS selectors can refer back to must be added to your HTML document.
2. CSS rules that select that code must be added to your style sheet.

The code for classes and IDs is different in both CSS and HTML.

## HTML code

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

Note that it's possible to assign more than one class to an element — just leave a blank space between the two classes, as in the baseball examples above.

Bonus: ID selectors can be used to create links that can be used for navigation *within* a page. For example, to add a link to the page that takes the user directly to the line that reads "New York Mets," we might write HTML like this: `<a href="#mets">Mets</a>`.

## CSS selectors

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

## ID selectors

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

*If you run into an error, be sure to check your punctuation. Oftentimes the problem is a typo, or overlooking a semi-colon, a period, etc.* See the [Troubleshooting](17-troubleshooting.md) section for more information on common issues.

# Useful Properties

Below is a list of useful properties that can be modified with CSS, compiled by Digital Fellow [Patrick Smyth](http://smythp.com). There are also [CSS cheatsheets](https://courses.cs.washington.edu/courses/cse154/15sp/cheat-sheets/css-cheat-sheet.pdf) available online.

## Color

Determines text color. Can be a word or a hex value, like #FFFFFF:

```css
color: blue;
color: #000000;
```

### Background color

Sets the background color of an element.

```css
background-color: pink
background-color: #F601F6;
```

### Text align

Aligns text to the left, center, or right.

```css
text-align: center;
```

### Padding

The space between text and the "box" (`<div>`) surrounding it.

```css
padding: 10px;
padding-right: 10px
```

### Margin

The space between an element's box and the next element (or the edge of the page).

```css
margin: 10px;
margin-top: 10px;
```

### Width and height

Sets the width or height of an element. Typically, don't set both of these.

```css
width: 50%;
height: 40px;
```

### Float

Determines if text wraps around an element.

```css
float: left;
```

### Display

Determines if an element is treated as a block or inline element. Can also be set to `none`, which makes the element disappear.

```css
display: inline;
display: block;
display: none;
```

### List style

Determines default styling on lists. Usually best to set it to `none`.

```css
list-style-type: none;
```

### Font family

Sets the font. Usually best to copy this from [Google Fonts](https://fonts.google.com/) or another web font repository.

```css
font-family: 'Lato', sans-serif;
```

# Challenge: Styling your Institute Website with CSS

Using the CSS basics we've just reviewed, and the list of properties found on the [Properties page](15-properties.md) and online, give your website some styling.

I encourage you to use an external stylesheet with classes and IDs to style particular aspects of your site more specifically, but feel free to also play around with inline and internal styling if desired.

## Challenge

- Change the color and size of your heading text.
- Change the font of your paragraph text.
- Change the background color of your navigation bar or menu.
- Center your image on your page.
- [Shape up your navigation bar.](_navbar-hint.md)

**Reminder:** After creating a stylesheet, you must link it to all HTML documents that you want this styling to apply to. You can do so with the `<link>` tag:

```html
<link rel="stylesheet" type="text/css" href="style.css" />
```

This will tell your HTML document to apply the style rules from the text file named `style.css` in the same folder.

# Troubleshooting

It is common—especially in the beginning—that you'll add or amend something to/in your text editor, but it won't present when rendered by your browser.

Your first inclination should be to scan the text in your editor for errors. Nesting will help tremendously with this task. Oftentimes it is as little as forgetting a semicolon or closing tag.

Another investigative tactic is to **View Page Source** on the page opened in the browser.

If you think it is an **error with the HTML**, you'll be able to see it there.

If you think it is an **error with the CSS**, then from the Page Source you'll need to click on the link for the `style.css` page. The link to this page should be found in the head of your page. Don't see it? That may be the problem! If you do see it, open the link to see what CSS the browser is reading and applying to your HTML. It should match what you have in your text editor. If it looks like an earlier version of your style sheet, then maybe you need to re-save the document.

# Workshop Summary

Through this workshop, you have learned the basics of two of the most commonly-used languages for building on the web: HTML and CSS.

HTML, or Hypertext Markup Language, organizes content on your page using [elements denoted by tags (`< >`)](04-elements.md). When rendered by your browser, these tags tell your browser that certain content is paragraph text, while other content is heading or title text, and so on. You can also use [image (`<img>`)](07-images.md) and [link or anchor (`<a>`)](06-links.md) tags to tell the browser to render an image on the page, or take the visitor to another page on your or another website. We also discussed some important [conventions](08-conventions.md) to consider when creating HTML documents, such as nesting.

CSS, or Cascading Style Sheets, allows for further styling of your website through the application of a series of [rule sets](12-rules.md) that are applied to different aspects/elements of your site. In order for CSS to render on a webpage, it must be [integrated with your html](11-integration.md), which can happen in three ways: inline, internal, and external. CSS rules can be of varying specificity, and in particular, through creating [classes and ids](14-classes.md). We also discussed how the ordering of rule sets doesn't matter, because an important function of CSS is the way it filters and applies rules in accordance with the specificity of the rule.

Through understanding these languages in combination with one another, you can also reframe your understanding of the web—not as _poof! magic!_, but as a series of intentionally styled, hyperlinked text documents, with each website representing a folder of documents.

While this is a good starting point, one important question remains: how can I get these text documents on the Internet so they can be accessed, and interacted with, and linked to by others?

# Making your Website Public

Great job! Now you have an amazing website, but it's stuck on your computer where no one else can find it or view it. How do you get your website onto the Internet so it can be shared?

To get your site on the internet, you'll need **hosting** — that is, a remote computer that will stay on day in and day out to serve the website to visitors. In theory, you could host your website on your own computer, but in practice, it usually makes sense to purchase hosting from a hosting company or use a free service.

You'll also need a way of getting your website to your host. That's where FTP, or File Transfer Protocol, comes in.

## FTP

FTP is a protocol used to share files from your computer (_a client_) to another computer called a server, and back again over the Internet. This is something we do ALL THE TIME, but we refer to it as "uploading" and "downloading."

Note: Though FTP stands for file transfer protocol, you are not really transfering or moving your files from your computer; instead they are _copied_ to the server. Fear not!

In order to transfer your website files (also called your website's directory) to a server you will need:

1. Access to the Internet.
2. An FTP Client.
3. A server that is connected to the Internet where you can send your files.

Assuming you all can manage accessing the internet on your own, let's focus on the latter two.

### FTP client

An **FTP client** is software designed specifically for the purpose of sharing files between computers. There are widely-used, freely-available GUI applications (i.e., applications that use a graphic user interface, or the point-and-click, user-friendly software interfaces you are used to) that you can download for use, including [Filezilla](https://filezilla-project.org/) and [Cyberduck](https://cyberduck.io/). You can also run an FTP client program through the command line on most computers, though the process varies by operating system.

### Other Resources about FTP

- [FTP for Beginners, *Wired*](https://www.wired.com/2010/02/ftp_for_beginners/)
- [The Three Best FTP Clients for Windows](https://www.makeuseof.com/tag/free-ftp-clients-windows/)
- [How To Use FTP Through the Command Line in Mac OS X](http://www.techradar.com/how-to/software/operating-systems/how-to-use-ftp-through-the-command-line-in-mac-os-x-1305664)
- [How to Use the Mac Terminal as an FTP or SFTP Client](https://beebom.com/how-to-use-mac-terminal-ftp-sftp-client/)

## Web hosting

You also need a server to transfer your files to, where they can be stored and shared on the Internet. This is what we call **web hosting** and there are multiple options here as well. The GCDI (CUNY Graduate Center Digital Initiatives) website contains a list of [low-cost cloud hosting services for students](https://gcdi.commons.gc.cuny.edu/digital-resource-guide/#cloud). As long as your site is just plain HTML and CSS, it's also possible to host your website for free on services such as [GitHub Pages](https://pages.github.com/).

### Web hosting services

- [The Best Web Hosting Services](https://www.makeuseof.com/tag/best-web-hosting-services/)
- [Top 7 Easy and Free Web Hosting Services](https://www.makeuseof.com/tag/top-7-easy-and-free-web-hosting-services/)
- [10 Ways That Free Web Hosting Is Bad for Your First Website](https://www.makeuseof.com/tag/free-web-hosting-is-bad/)

# Resources

## Cheatsheets

[HTML Cheatsheet](http://www.simplehtmlguide.com/cheatsheet.php)  
[CSS Cheatsheet](https://courses.cs.washington.edu/courses/cse154/15sp/cheat-sheets/css-cheat-sheet.pdf)  

## Tutorials

[HTML Tutorial](https://www.w3schools.com/html/default.asp)  
[CSS Tutorial](https://www.w3schools.com/css/default.asp)  

## Other

[Code School's Beginner's Guide to Web Development](https://www.codeschool.com/beginners-guide-to-web-development)  
[Web Development with Accessibility in Mind](https://www.w3.org/standards/webdesign/accessibility)  
[Web Design Inspiration](https://www.webdesign-inspiration.com/)  
[YouTube Series: How to Build a Responsive Website from Start to Finish](https://www.youtube.com/playlist?annotation_id=annotation_698551941&feature=iv&list=PLqGj3iMvMa4KQZUkRjfwMmTq_f1fbxerI&src_vid=WX0MpDuUqqw)   

