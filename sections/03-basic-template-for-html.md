← [Opening Activity](02-opening-activity.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Tags and Elements](04-tags-and-elements.md) →

---

# 3. Basic Template for HTML

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

Create a folder called `htmlpractice` in your projects folder (`~/Desktop/projects/htmlpractice`). Inside that folder, create a new text file and save it as `index.html`.

Let's use the command line to create the new folder and file:

1. Open your terminal.
2. Navigate to your projects folder using this command:

    ```console
    $ cd ~/Desktop/projects
    ```

3. Create a new folder:

    ```console
    $ mkdir htmlpractice
    ```

4. Use your Visual Studio Code text editor to create a file called `index.html`: `code index.html`.
5. Paste the template above (starting with `<!DOCTYPE html>`) into the new file.

The `index.html` file is your default homepage for the website we are creating. This is an industry standard, because web browsers tend to recognize the `index.html` page as the opening page to the directory that is your website. See [here](https://www.lifewire.com/index-html-page-3466505) for more explanation.

Once you've created your new file, open it with a web browser using your graphical user interface:

On macOS, click on the Finder in your dock (the apps at the bottom of the screen) and click on Desktop on the left. From there, navigate to `projects`, then `htmlpractice`. Alternately, you can click the projects folder icon on your Desktop and find it from there. If you're using a Mac and would prefer to use the command line, you can also type `open index.html` from within your `htmlpractice` folder.

On Windows, click the `projects` folder icon on your desktop. Navigate to `projects`, then `htmlpractice`. Double click the `index.html` file. If it does not open in a browser, right click the `index.html` icon and select "Open with..." from the menu. Select Firefox or Google Chrome from the app list that appears.

## What Happens?

When you open the empty template, you'll see only a blank web page. Open your secondary menu (right click on Windows, hold <kbd>control</kbd> and click with macOS) and view the page source.

## What Should Happen When I Open Each of my Two New Files?

When you "View Page Source," you should see the code for the basic template.

No content renders on the page, because there is no content in the template at this time.

## Evaluation

Which of these two HTML commands is also known as the "root element"?
- `<!DOCTYPE html>`
- `<html lang="en">`*

## Keywords

Do you remember the glossary terms from this section?

- [Root Element](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/rootelement.md)

---

← [Opening Activity](02-opening-activity.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Tags and Elements](04-tags-and-elements.md) →