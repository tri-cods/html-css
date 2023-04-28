[<<<Back](18-summary.md) | [Next>>>](20-resource.md)

# Making your Website Public

Great job! Now you have an amazing website, but it's stuck on your computer where no one else can find it or view it. How do you get your website onto the Internet so it can be shared?

To get your site on the internet, you'll need **web hosting** — that is, a remote computer or **server** that will stay on day in and day out to serve the website to visitors. In theory, you could host your website on your own computer, but in practice, it usually makes sense to purchase hosting from a hosting company or use a free service. There are many options for hosting: we're going to focus on using shared hosting accounts from [Reclaim Hosting](https://reclaimhosting.com/), which each of the Tri-Colleges provides through a campus-wide Domain of One's Own service.

## Domain of One's Own

To create a new account or log into your existing account, follow the URL for your College: 
- Bryn Mawr's Domain of One's Own: https://digital.brynmawr.edu
- Haverford Sites: https://sites.haverford.edu/
- Swarthmore Domains: https://domains.swarthmore.edu/

Take note of the URL for your institution, because in fact your website will be a **subdomain** of that subdomain, which means it will be included in your website's URL.

- The subdomain you chose: e.g. `alice`
- The subdomain for your school's webhosting service: `digital`
- Your school's root domain: `brynmawr.edu`

In this case, the URL for my domain's account is: `alice.digital.brynmawr.edu`

When you log into your account, you'll see the **cPanel Dashboard**, which allows you to customize your hosting space, install web applications, and manage all aspects of this hosting account. From your dashboard you can access the **File Manager**, which offers a graphic user interface for navigating the documents, software, and data stored on your hosting account (just as your local computer's operating system allows you to view and manage documents and files). Within the root directory of your domain you'll see the **public_html** folder: this folder contains any public-facing content served from your domain.

While today we'll focus on deploying your hand-coded html sites, your webhosting account also provides many other options for creating digital projects and websites. From the Dashboard you can access the **applications** menu, which you can use to install and manage open-source **content management systems** such as WordPress, Omeka, or Scalar. To learn more about these options, see your school's Domain of One's Own documentation. No matter what tool you use, your skill with HTML and CSS will come in handy as you customize the style and content of your website.

## Activity: publishing your site on Domain of One's Own

1. Compress the folder containing your website and its assets (html, css, and images)
   - On a Mac: in Finder, select the folder and right click to open the secondary menu. Select 'Compress folder'
   - On Windows: press and hold or right-click the folder and select Send to > Compressed (zipped) folder
2. From your Domain of One's Own dashboard, open the File Manager and navigate to the public_html directory
3. Upload the compressed file and extract it into your public_html directory. This should create a subdirectory named 'htmlpractice' (or whatever you named that folder initially) that contains your `index.html` file and other assets it refers to.
4. The web address for your new site will be the url for your domain of one's own account followed by a backslash and the name of the subdirectory containing your site files:  `alice.digital.brynmawr.edu/htmlpractice` 
5. Open a separate browser or tab and navigate to this URL to see your site live on the web!

### Other web hosting services

The GCDI (CUNY Graduate Center Digital Initiatives) website contains a list of [low-cost cloud hosting services for students](https://gcdi.commons.gc.cuny.edu/digital-resource-guide/#cloud). As long as your site is just plain HTML and CSS, it's also possible to host your website for free on services such as [GitHub Pages](https://pages.github.com/).

- [The Best Web Hosting Services](https://www.makeuseof.com/tag/best-web-hosting-services/)
- [Top 7 Easy and Free Web Hosting Services](https://www.makeuseof.com/tag/top-7-easy-and-free-web-hosting-services/)
- [10 Ways That Free Web Hosting Is Bad for Your First Website](https://www.makeuseof.com/tag/free-web-hosting-is-bad/)

[<<<Back](18-summary.md) | [Next>>>](20-resource.md)
