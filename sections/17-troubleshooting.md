[<<<Back](16-creating_stylesheet.md) | [Next>>>](18-summary.md)

# Troubleshooting

It is common—especially in the beginning—that you'll add or amend something to/in your text editor, but it won't present when rendered by your browser.

Your first inclination should be to scan the text in your editor for errors. Nesting will help tremendously with this task. Oftentimes it is as little as forgetting a semicolon or closing tag.

Another investigative tactic is to **View Page Source** on the page opened in the browser (just like we did in our [opening activity](02-opening_activity.md))

If you think it is an **error with the HTML**, you'll be able to see it there.

If you think it is an **error with the CSS**, then from the Page Source you'll need to click on the link for the `style.css` page. The link to this page should be found in the head of your page. Don't see it? That may be the problem! If you do see it, open the link to see what CSS the browser is reading and applying to your HTML. It should match what you have in your text editor. If it looks like an earlier version of your style sheet, then maybe you need to re-save the document.

Many browsers also have **Web Inspector** or other **Developer Tools** that will let you see the HTML and CSS that make up specific parts of the page.

1. Open a web browser (Firefox, Chrome, or another Chromium-based browser works best).
2. Select an element with your cursor. 
3. Open the secondary menu (using a mouse, this would be the menu that opens when you right click on the page; on Mac computers, this is usually a two-finger tap on the track pad, or you can press the "control" button then click the track pad).
4. Select 'Inspect'

You'll usually see a split-screen that will show you the HTML for that element highlighted. In many cases you can expand or minimize different nested elements within the html document.

Another pane will show the CSS rules that apply to that particular element. You'll notice that some of these rules may be crossed out -- that's because they are rules that apply to that element but are overridden by other rules. You may even see the filename and line number of the relevant CSS. This can be very helpful if you're attempting to customize a web page developed by someone else.

[<<<Back](16-creating_stylesheet.md) | [Next>>>](18-summary.md)
