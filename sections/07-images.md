[<<<Back](06-links.md) | [Next>>>](08-conventions.md)

# Images

Images are another important component of websites. Sometimes these just help bring your website to life, but other times they can help communicate information to users.

Images are created with the `<img/>` tag. Similar to the `<a>` tag, `<img>` requires an attribute with a link, in this case `src`. The `src` attribute stands for "source" and communicates secondary information to your browser that identifies and locates the image. Unlike many other tags, the `<img>` tag does not need to be closed, making it an example of a void tag.

The following element pulls in an image located in the same folder as the `.html` file:

```html
<img src="scream.jpeg" />
```

The same rules apply here as with the `href` attribute: if the image is not located in the same folder as the document you are writing in, the browser won't find it. If the browser cannot find an image resource, you will see a broken image icon, such as this one from Chrome:

![Chrome broken image icon](images/broken.png)

Note: Some sites use a lot of images. When this is the case, it can be helpful to keep images in a separate folder within your site's structure. To enable the browser to find an image in that case, just add the directory in front of the file name. For example, if you have a folder named images in the same folder as your index.html file, and scream.jpeg is in that folder, you'd change the void tag above to `<img src="/images/scream.jpeg" />`.

Also like `href`, the `src` attribute can link to an image hosted elsewhere on the web, as long as it is a direct url ending with an image filename and file extension.

## Making images accessible

As briefly noted earlier, alternative text provides a description of an image's basic function or content and it is necessary to make your website accessible to all users. While some users navigate the web visually with traditional browsers, many users navigate with screen reader software that conveys all information aurally by reading text and image descriptions. Other users with low-bandwith internet may opt to display alternative text instead of data-intensive images. 

The most common way to include alternative text is to add an `alt` attribute to an image element, followed by your descriptive text. For example:

```html
<img src="filename.png" alt="Text in these quotes describes the image" />
```

If an image is purely decorative and has no semantic function, you can include a null alt attribute with empty quotation marks `alt=""`, which signals to screen readers that the content is not significant. For more information, see the [Wikipedia Manual of Style/Accessibility/Alternative Text for Images](https://en.wikipedia.org/wiki/Wikipedia:Manual_of_Style/Accessibility/Alternative_text_for_images) and the [Social Security Administration's guide to alternative text](https://www.ssa.gov/accessibility/files/SSA_Alternative_Text_Guide.pdf) has to say.

## What images can I use on my site?

If you're planning to use images that you did not take or make yourself, you'll need to use "public domain" or "open license" images.

This [guide by the OpenLab at City Tech](https://openlab.citytech.cuny.edu/blog/help/following-copyright-guidelines-for-images/) includes more information on licensure and a list of places where you can find reuseable images.

## Activity

Download and save an image from the web, or move an image from your computer into the same folder as your `index.html` file.

Tip: Give the file a simple name. Also, the name **cannot** have spaces. A good practice is to use either dashes or underscores where there would otherwise be spaces. For example: `this-is-an-image.jpg` or `this_is_an_image.jpg`.

Using the code above as a reference, add that image into your `index.html` file, re-save the file, and re-open or refresh the page in your browser. Your image should now appear on the page.

[<<<Back](06-links.md) | [Next>>>](08-conventions.md)
