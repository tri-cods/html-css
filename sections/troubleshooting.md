[<<<Back](creating_stylesheet.md) | [Next>>>](summary.md)

# Troubleshooting

It is common — especially in the beginning — that you'll add or amend something to/in your text editor, but it won't present when rendered by your browser.

Your first inclination should be to scan the text in your editor for errors. Nesting will help tremendously with this task. Oftentimes it is as little as forgetting a semicolon or closing tag.

Another investigative tactic is to **View Page Source** on the page opened in the browser.

If you think it is an **error with the HTML**, you'll be able to see it there.

If you think it is an **error with the CSS**, then from the Page Source you'll need to click on the link for the `style.css` page. The link to this page should be found in the head of your page. Don't see it? That may be the problem! If you do see it, open the link to see what CSS the browser is reading and applying to your HTML. It should match what you have in your text editor. If it looks like an earlier version of your style sheet, then maybe you need to re-save the document.

[<<<Back](creating_stylesheet.md) | [Next>>>](public.md)