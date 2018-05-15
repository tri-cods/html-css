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

Within the root element of the basic template below, you'll notice the two main sections of all HTML documents - a head section (demarcated by `<head>` and `</head>`) and a body section (demarcated by `<body>` and `</body>`). 

The **head section** contains basic information about the file such as the title, keywords, authors, a short description, etc. This is also where you will link to your CSS stylesheet which describes how you want the page styled (what color, font, size of text, where and how do you want the cotent laid out, etc—something we'll talk about later.

The **body section** contains the content of the page including paragraphs, images, links, and more, and indicates how this content is to be structured on the page. 

## Activity

Create a folder called `html_css` on your desktop.

**CHALLENGE** Use the command line to do it. 

1. Open your terminal
2. Navigate to your desktop
3. Create a new folder called "website"
4. Create a new file in that folder called index.html. 
5. Create a second new file in that folder called about.html.
(See below for commands.)

Open your text editor (Visual Studio Code) and open your two newly created files (index.html and about.html).

Type or copy and paste the template above into your two new text files and resave.

These are the first two pages of your new website! 

*Note: The `index.html` file is your default homepage. This is an industry standard, because web browsers tend to recognize the `index.html` page as the opening page to the directory that is your website.* See [Resources](resource.md) for more.

Once you have both documents saved, open them by
A. Opening your file manager (i.e. Finder on Macs)
B. From the command line, make sure you are in the same folder as the file, and type open `index.html`.

What happens? 

Open your secondary and view the page source. How can you explain what happens when you open these text files? 
<br/>
<br/>
<br/>

## Command line to Create New files
After opening your terminal, you:
2. $ cd Desktop
3. $ mkdir website
4. $ mkdir website 
   $ touch index.html
5. $ touch about.html

## What should happen when I open my two new files?
A blank page should open in your web browser. 

When you 'View Page Source', you should see the code for the basic template. 

No content renders on the page, because there is no coontent in the template at this time. 

[<<<Back](opening_activity.md) | [Next>>>](elements.md)
