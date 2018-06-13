[<<<Back](opening_activity.md) | [Next>>>](elements.md)

# Basic Template for HTML

Below is a basic template for an empty HTML Document. 

```
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

The root element begins by indicating which language the document is written in; and in this basic template, `en` tells us and the computer that we are writing in English. 

Within the root element of the basic template below, you'll notice the two main sections of all HTML documents: a head section (demarcated by `<head>` and `</head>`) and a body section (demarcated by `<body>` and `</body>`). 

The **head section** contains basic information about the file such as the title, keywords, authors, a short description, and so on. This is also where you will link to your CSS stylesheet which describes how you want the page styled—what color, font, size of text, and positioning of elements on the page.

The **body section** contains the content of the page, including paragraphs, images, links, and more, and indicates how this content is to be structured on the page. 
## Activity

Create a folder called `htmlpractice` in your projects folder (`~/Desktop/projects/htmlpractice`). If you haven't created a projects folder in an earlier session, create a folder on your desktop instead. Inside that folder, create two new text files: `index.html` and `about.html`.

Let's use the command line to create the new folder and files:

1. Open your terminal.
2. Navigate to your projects folder using this command: `cd ~/Desktop/projects`.
3. Create a new folder: `mkdir htmlpractice`.
4. Use your VS Code text editor to create a file called `index.html`: `code index.html`.
5. Paste the template above (starting with `<!DOCTYPE html>`) into the new file.
6. Repeat to create a text file titled `about.html`

The `index.html` file is your default homepage for the website we are creating. This is an industry standard, because web browsers tend to recognize the `index.html` page as the opening page to the directory that is your website. See [here](https://www.lifewire.com/index-html-page-3466505) for more explanation.

Once you've created your new files, open them with a web browser using your graphical user interface:

On Mac OS, click on the Finder in your dock (the apps at the bottom of the screen) and click on Desktop on the left. From there, navigate to `projects`, then `htmlpractice`. Alternately, you can click the projects folder icon on your Desktop and find it from there. If you're on Mac and would prefer to use the command line, you can also type `open index.html` from within your `htmlpractice` folder.

On Windows, click the `projects` folder icon on your desktop. Navigate to `projects`, then `htmlpractice`. Double click the `index.html` file. If it does not open in a browser, right click the `index.html` icon and select `Open with...` from the menu. Select Firefox or Google Chrome from the app list that appears.

### What happens?

When you open the empty template, you'll see only a blank web page. Open your secondary menu (right click on Windows, hold control and click with Mac OS) and view the page source. How can you explain what happens when you open these text files? 

## What should happen when I open each of my two new files?

When you 'View Page Source', you should see the code for the basic template. 

No content renders on the page, because there is no content in the template at this time. 

[<<<Back](opening_activity.md) | [Next>>>](elements.md)
