##Introduction
This template utilizes Jekyll, an open source static website generator, as well as a theme based largely off of the Minimal Mistakes theme by Michael Rose. The purpose of this template is to provide you with a simple, well designed website that is optimized for hosting on Github pages. We aim to reduce the technological know-how and time that is usually required for maintaining a personal or professional website.

####Why Should I Use This?
By using this template you will have a website that is well designed, easy to maintain, free to host and easy to update. While there are many options out there for personal and professional websites, most are dependant on the platform on which they were built, and cannot be easily migrated. This template, while built for Github Pages integration, provides flexibility should you choose to host it elsewhere.

##First Steps
In order to get started you will need to first create your own Github account by going to [github.com](https://github.com/). Your username will be part of your site's URL, so choose wisely. You will be prompted to choose an account type, choose the Free account option. After creating your account you will need to create a new repository. **You must name your repository [username].github.io** (replacing [username] with the username of your Github account). If you have any troubles creating a repository please refer to the [Github Pages](https://pages.github.com/) documentation.


![Create a Repository] (https://github.com/toddstoffer/jekyll-academic/blob/master/%20createrepo.gif)

####Copying the Template
Once you have created your new repository you will be taken to a setup page. At the bottom of that page you should see the **Import Code** button. Click on this button. The following page has a place for you to put the URL of an existing repository, copy and paste the following into that space:
`https://github.com/gwu-libraries/jekyll-academic`

After the import is complete you can then visit [username].github.io and you will see your newly created website. On this page you will see a variety of posts that contain more detailed information on editing, modifying and updating your new website.

##Next Steps
After you have imported the files into your repository, you'll need to personalize them. You can use the "edit this file" button, which looks like a pencil, to edit the files. 

####Editing the \_config.yml File
The \_config.yml file that is in the root directory of the project is the first file that you will want to edit. This file allows you to set the website title, your email address and add in account information for a variety of social media services. Only the options you fill out will appear on the main page. 

When you're done with your changes, you "commit changes " to them. This is like saving the file to the repository. Add a brief commit message, for example "updating colors", and click the green "Commit changes" button. 

####Editing the accent.scss File
The accent.scss file allows you to modify the accent colors of your website. The default colors (red and black) can be set to any hexadecimal color that you would like. [W3Schools.com](http://www.w3schools.com/colors/colors_picker.asp) provides a good color picker that allows you to find the corresponding hex number for any color you wish to use.

####Editing the About Me and Resume Pages
These pages are each found in their corresponding directories (/about /resume). Simply edit the index.md file in each of these directories. Pay special attention to the formatting of the resume file. It makes use of single quotes ( \' ) and underscores ( \_ ) in the markdown markup language to format various aspects of the resume, including dates and university names.

When you are done "Commit changes" to save them. 

These pages are formatted using Markdown. [Markdown Cheat Sheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)

####Adding a bio image and a logo
images/bio-photo.jpg - This is the photo that appears on the home page of the website. The recommended image size is 200px x 200px. To use your own image:
1. Click the gray "Upload files" button at the top of the file list in Github and select your image file to upload.
2. Go to the \_config.yml file and edit it. Change the "avatar" field to your uploaded image filename. 

images/logo.png - If you wish to use a logo for your site, upload a logo file into the images folder. You will also need to add logo.png under the 'Logo:' section of the \_config.yml file.

\_data/navigation.yml -This is the file that allows you to manage your navigation elements. By default all available navigation items are shown. If you wish to hide any items, simply delete them from this file.


####Editing Blog Posts
Blog Posts are all located in the \_posts folder. This folder contains sample posts that address in more depth the site structure and the markdown syntax. These posts are good to reference (by opening in a text editor of your choice) in order to get a better understanding of markdown. When you are ready to add a new post, simply copy one of the existing posts and edit it. Be sure to update the information at the top of the post, such as the title and timestamp. You will also want to rename the file to follow the same naming convention of the other post files (yyyy-mm-dd-post-title.md).

##Viewing Your Changes
Edits to your files should show up within a minute or two. Go to [username].github.io to view them. 

##Problems?
If your changes aren't showing up on the site, it's possible that there's a problem building your site.  You can go to your Github repository's Settings page and scroll down to the GitHub Pages section (on the Options tab).  If all is well, this section should say "Your site is ready to be published at https://[username].github.io/."  If there's a problem, it will say something similar to: "Your site is having problems building" and should also tell you which line of which file is causing the error.
