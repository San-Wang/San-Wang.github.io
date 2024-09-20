# [Portfolio Website](https://san-wang.github.io)  

Powered by Jekyll Academic, developed by NCSU Libraries, a template utilizes Jekyll, as well as a theme based largely off of the Minimal Mistakes theme by Michael Rose. Its features include the ability to create blog posts, a dedicated resume page, social media integration and the ability to create and host Reveal.js presentations. It is also designed to be hosted on GitHub pages.

Thanks:  
GWU Libraries workshop "[Build a Professional Website With GitHub Pages](https://library.gwu.edu/news-events/events/build-professional-website-github-pages%E2%80%8B)"

Site Structure:
Contain profile, resume, projects, blogs.  
```
---------------------------------------------------
Low Risk:
├── index.md
├── resume.md
├── _config.yml
|
├── _posts
│   └── YYYY-MM-DD-title.md
|
├── images
│   ├── bio-photo.jpg
│   └── logo.png
├── _data
│   └── navigation.yml
---------------------------------------------------
Medium Risk:
├── _sass
│       
├── _includes
│   ├── _author-bio.html
│   ├── _browser-upgrade.html
│   ├── _cvhead.html
│   ├── _disqus_comments.html
│   ├── _feed-footer.html
│   ├── _footer.html
│   ├── _head.html
│   ├── _navigation.html
│   ├── _open-graph.html
│   ├── _scripts.html
│   ├── _social-share.html
│   └── _toc.html
├── _layouts
│   ├── home.html
│   ├── page.html
│   ├── post-index.html
│   ├── post.html
│   ├── presentation-post-index.html
│   ├── resume.html
│   └── slide.html
├── assets 
│ 
---------------------------------------------------
High Risk:
├── favicon.png
├── presentations.md
├── blog.md
├── 404.md
├── Gemfile
├── Gemfile.lock
├── Gruntfile.js
├── LICENSE
├── README.md
```

References:  
* Jekyll academic workshop handout.pdf provided by GWU library
* [Site structure with risky levels](https://ncsu-libraries.github.io/jekyll-academic-docs/advanced/#using-jekyll-locally)
* [Jekyll Academic](https://ncsu-libraries.github.io/jekyll-academic-docs/documentation/)[(github)](https://github.com/NCSU-Libraries/jekyll-academic)  
* [Minimal Mistakes Theme](https://mmistakes.github.io/minimal-mistakes/)
* [Jekyll Resources](https://jekyllrb.com/resources/)
