[<<<Back](18-summary.md) | [Next>>>](20-resource.md)

# Making your Website Public

Great job! Now you have an amazing website, but it's stuck on your computer where no one else can find it or view it. How do you get your website onto the Internet so it can be shared?

To get your site on the internet, you'll need **web hosting** — that is, a remote computer or **server** that will stay on day in and day out to serve the website to visitors. In theory, you could host your website on your own computer, but in practice, it usually makes sense to purchase hosting from a hosting company or use a free service. There are many options for hosting: we're going to focus on using shared hosting accounts from [Reclaim Hosting](https://reclaimhosting.com/), which each of the tri-colleges provides for users through a campus-wide Domain of One's Own service.

## Domain of One's Own

While today we'll focus on deploying your hand-coded sites, your webhosting account allows you to explore other options, including **content management systems**  that can be installed on your account such as WordPress, Omeka, Scalar, and many more.

To create a new account or log into your existing account, follow the URL for your College: 
- Bryn Mawr's Domain of One's Own: https://digital.brynmawr.edu
- Haverford Sites: https://sites.haverford.edu/
- Swarthmore Domain of One's Own: 

Take note of the URL for your institution, because in fact your website will be a **subdomain** of that subdomain, which means it will be included in your website's URL.

- The subdomain you chose: e.g. `alice`
- The subdomain for your school's webhosting service: `digital`
- Your school's root domain: `brynmawr.edu`

In this case, the URL for my website is: `alice.digital.brynmawr.edu`

### cPanel Dashboard

### File Manager

The File Manager is the way you can directly see the software and data stored on your account. Public content for your main domain will go in your **public_html** folder. This is where you can upload files to be served on your site.

1. Zip up the folder containing your website and its assets (html, css, and images)
2. Navigate to public_html in the file manager
3. Upload the compressed file and extract it into your public_html folder.
4. In a separate browser window, navigate to your domain's url (alice.digital.brynmawr.edu)
5. Add /site to the end to see your files live on the web!


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

### Other web hosting services

The GCDI (CUNY Graduate Center Digital Initiatives) website contains a list of [low-cost cloud hosting services for students](https://gcdi.commons.gc.cuny.edu/digital-resource-guide/#cloud). As long as your site is just plain HTML and CSS, it's also possible to host your website for free on services such as [GitHub Pages](https://pages.github.com/).

- [The Best Web Hosting Services](https://www.makeuseof.com/tag/best-web-hosting-services/)
- [Top 7 Easy and Free Web Hosting Services](https://www.makeuseof.com/tag/top-7-easy-and-free-web-hosting-services/)
- [10 Ways That Free Web Hosting Is Bad for Your First Website](https://www.makeuseof.com/tag/free-web-hosting-is-bad/)

[<<<Back](18-summary.md) | [Next>>>](20-resource.md)
