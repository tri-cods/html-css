[<<<Back](p_and_h.md) | [Next>>>](images.md)

# Links

Links are another important component of most websites. By hyperlinking text, you can move between the different webpages on your site (sometimes in the form of a menu or navigation bar), or connect to other resources or information on other websites.

The `<a>` tag, or **anchor tag**, creates the link to another document. You can use the `<a>` tag to link to other documents or webpages you created for the same site or to documents or webpages created by other web users. 

## OPTION 1: Linking to your own documents

The following appears as a link to the `about.html` page on the same site: 

```
<a href="about.html">About</a>
```

On your webpage it will appear as:

[About](about.html)  

By adding this to your `index.html` file, this pathway is asking the browser to look for a file titled `about.html` in the same folder. And the pathway in the code above is asking the browser to look in the same folder as the `index.html` file. If these are not in the same folder, this link will not work. 

## OPTION 2: Linking to other webpages/websites

```
<a href="http://www.google.com">Google</a>
```

On your webpage it will appears as:

<a href="http://www.google.com">Google </a>

This pathway is directing your browser to look online for this text document at the URL address provided.

Each example above also includes an `href` tag. The `href` tag, short for hypertext reference, is an example of an **attribute**. Attributes offer secondary information to your browser. 

In reading the anchor element in the examples above, the `<a>` tag, which indicates that the following text will include a link to another document. This is the primary information your browser takes in. The `href` tag tells your browers where the document can be found. This secondary information.

There is another technical difference between the two options above.
<ul> 
	<li> Option 1 is called a **relative link** because the link  describes the URL in relation to the page you're on. </li>
	<li> Option 2 is called an `absolute` link because it describes the URL as a separate entity, requiring that the the whole URL be included. </li>
</ul>

## Best Practice Tip: 
Use relative links when referring to pages on your own site; in other words, in the href section, tell your browser it can find that document in the same folder as the document it is currently reading. This is a preventative measure that will prevent links on your site from breaking should you decide to move your site.

## ACTIVITY:
In your `index.html` file, add a relative link to your About page. 
<br/>
<br/>
Re-save that document and re-open it in your broswer - you can refresh the page if you still have it open, or re-open it through the finder.

Also add a relative link from your `About page` to your `index.html` page. Call this page `Home`. This will allow you to toggle back-and-forth between the two pages.

Lastly, include an absolute link to a page of your choosing.
<br/>
<br/>

[<<<Back](p_and_h.md) | [Next>>>](images.md)