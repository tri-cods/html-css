[<<<Back](02-opening_activity.md) | [Next>>>](04-elements.md)

# Anatomy of an HTML Document

You can think of an HTML document as a tree with branches that decrease in size. Each branch is demarcated by a set of nearly identical opening `<html>` and closing `</html>` tags. This is the basic structure of that tree:

```html
<!DOCTYPE html>
<html lang="en">
    <head>
    </head>
    <body>
    </body>
</html>
```

HTML documents start with a `DOCTYPE` declaration that states what version of HTML is being used. This tells the browser how to read the code below it to render the page. If the webpage were written with a different markup language (i.e. XML, XHTML), it would tell you here.

After the `DOCTYPE`, we see the start of the **Root Element**. EVERYTHING—all content—that you want presented on this page and all information about how you want that information to be organized and styled goes in the root element, and it is demarcated by `<html>` and `</html>`.

The root element begins by indicating which language the document is written in. In this basic template, `lang='en'` tells us and the computer that text will be English. Documents without this tag will still display, but the omission could cause accessibility challenges for users who rely on assistive technology or in-browser translation. 

Within the root element of the basic template above, you'll notice the two main sections of all HTML documents: a head section (demarcated by `<head>` and `</head>`) and a body section (demarcated by `<body>` and `</body>`).

The **head** branch contains basic metadata about the file such as the title, keywords, authors, a short description, and so on. None of this metadata will appear on the webpage itself (though the title here will appear in your browser tab), but it provides instructions and context for your browser. This is also where you will link to external resources such as CSS files.

The **body** branch contains all the content to be displayed on the page, including paragraphs, images, links, and more, and indicates how this content is to be structured on the page.


## To start

Create a folder called `htmlpractice` in your projects folder (`~/Desktop/projects/htmlpractice`). If you haven't created a projects folder in an earlier session, you can create one now. Inside that folder, create a new text file and save it as `index.html`.

1. Use your VS Code text editor to create a file called `index.html`.
2. Type the template above (starting with `<!DOCTYPE html>`) into the new file. 

The `index.html` file is the homepage for the website we are creating -- the name 'index' is conventionally used to refer to the opening page to the directory that is your website. See [here](https://www.lifewire.com/index-html-page-3466505) for more explanation.

Once you've created your new file and saved that content, open it with a web browser using your graphical user interface:

On macOS, click on the Finder in your dock (the apps at the bottom of the screen) and click on Desktop on the left. From there, navigate to `htmlpractice`. Alternately, you can click the `htmlpractice`folder icon on your Desktop and find it from there. If you're using a Mac and would prefer to use the command line, you can also type `open index.html` from within your `htmlpractice` folder.

On Windows, click the `htmlpractice` folder icon on your desktop. Double click the `index.html` file. If it does not open in a browser, right click the `index.html` icon and select "Open with..." from the menu. Select Firefox or Google Chrome from the app list that appears.

### What happens?

When you open the empty template, you'll see only a blank web page. Open your secondary menu (right click on Windows, hold control and click with macOS) and view the page source. How can you explain what happens when you open these text files?

## What should happen when I open each of my two new files?

When you "View Page Source," you should see the code for the basic template.

No content renders on the page, because there is no content in your document at this time.

[<<<Back](02-opening_activity.md) | [Next>>>](04-elements.md)
