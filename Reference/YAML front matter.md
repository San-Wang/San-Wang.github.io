[YAML](http://yaml.org/) stands for YAML Ain't Markup Language. Markdown with [Front Matter](https://jekyllrb.com/docs/frontmatter/) placed at the front processed by Jekyll as a special file.   

Blog post naming convention: yyyy-mm-dd-title.md  
Blog post front matter template:  
```
---
layout: post
title: title
excerpt: "original serve as abstract, I use it to display tags underneath blog title"
excerpt: "tags - sub"
modified: yyyy-mm-dd 20:41:38
tags: [Machine Learning, Visualization, Articles, Recommendation System]
comments: true
category: blog
---  

Content start without title  
```
[front matter reference](https://ncsu-libraries.github.io/jekyll-academic-docs/documentation/)  

Tags tree:
```
|-- Visualization
|-- Articles
|-- Recommendation System
|-- Machine Learning
|   |-- Computer Vision
|       |-- Image Classification
|       |-- Image Segementation
|   |-- NLP
```

Features want to add in the future:  
* [ ] [Table of Contents](https://mmistakes.github.io/minimal-mistakes/docs/layouts/)  
```
---
toc: true
toc_label: "My Table of Contents"
toc_icon: "cog"
---
```

* [ ] Tags

