---
layout: post
title: Embed Tableau dashboard into github page post
excerpt: "Visualization - Tableau"
modified: 07/13/2018
tags: [Visualization, Tableau]
comments: true
category: blog
---  

Purpose of this article:  
After spending a lot of time searching online on how to embed tableau dashboard into my blog, I figure it would save people who want to do the same thing as me some time if I post my finding here. I will put the code I tried with the result that the dashboard showed in my blog together. 

## Preview  
>1. Basic embed code  
>2. Adjust iframe size  
>3. Hide "Tableau Public" redundant part
>4. Seamless iframe  
>5. Auto fit Tableau dashboard with iframe size  
>6. Adjust iframe size for moible view

[x] adjust iframe size
[x] hide Tableau software redundant part
[x] seamless 
[x] auto-fit dashboard within iframe
[] adjust iframe for mobile view


## 1. Basic embed code:  

Works fine on a regular whole page size website, but not suitable for my github page website.

~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=yes&:display_count=yes"></iframe>
~~~  
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=yes&:display_count=yes"></iframe>



## 2. Adjust iframe size:    

~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=yes&:display_count=yes" width = '650' height = '450'></iframe>
~~~   
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=yes&:display_count=yes" width = '650' height = '450'></iframe>  



## 3. Hide "Tableau Public" redundant part :  

~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=yes&:display_count=yes&:showVizHome=no" width = '650' height = '450'></iframe>
~~~  
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=yes&:display_count=yes&:showVizHome=no" width = '650' height = '450'></iframe> 


## 4. Seamless iframe:

~~~ ruby
<iframe seamless frameborder="0" src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=yes&:display_count=yes&:showVizHome=no" width = '650' height = '450'></iframe> 
~~~  
<iframe seamless frameborder="0" src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=yes&:display_count=yes&:showVizHome=no" width = '650' height = '450'></iframe> 


## 5. Automatically adjust tableau dashboard to make it fit within the iframe  

Share the same embed code as above, but a previous action required:  
Enable to use auto scale, need to set dashboard size as auto in Tableau Desktop!

~~~ ruby
<iframe seamless frameborder="0" src="https://public.tableau.com/views/GTSRB_Viz/GTSRB?:embed=yes&:display_count=yes&:showVizHome=no" width = '650' height = '450' scrolling='yes' ></iframe>    
~~~  

<iframe seamless frameborder="0" src="https://public.tableau.com/views/GTSRB_Viz/GTSRB?:embed=yes&:display_count=yes&:showVizHome=no" width = '650' height = '450' scrolling='yes' ></iframe>    

## 6. Adjust iframe size for moible view  

Exploring...
* JS way (researching)
You can't run HTML/JS in markdown files, simply because markdown is not actually anything that understands how to run HTML/JS. The only reason your markdown files are rendering correctly is because Jekyll is parsing your markdown files and rendering them as HTML/JS behind the scenes.
* iframe way

---
test
---  

<iframe seamless frameborder="0" src="https://public.tableau.com/views/GTSRB_Viz/GTSRB?:embed=yes&:display_count=yes&:showVizHome=no" width = 100% height = '450' scrolling='yes' ></iframe>     

.intrinsic-container {
  position: relative;
  height: 0;
  overflow: hidden;
}
 
/* 16x9 Aspect Ratio */
.intrinsic-container-16x9 {
  padding-bottom: 56.25%;
}
 
/* 4x3 Aspect Ratio */
.intrinsic-container-4x3 {
  padding-bottom: 75%;
}
 
.intrinsic-container iframe {
  position: absolute;
  top:0;
  left: 0;
  width: 100%;
  height: 100%;
}

<div class="intrinsic-container intrinsic-container-16x9">
  <iframe seamless frameborder="0" src="https://public.tableau.com/views/GTSRB_Viz/GTSRB?:embed=yes&:display_count=yes&:showVizHome=no" width = 100% height = '450' scrolling='yes' ></iframe> 
</div>

_________________________
[Reference](http://kb.tableau.com/articles/howto/embedding-tableau-public-views-in-iframes)  
[Parameters for Embed Code](https://onlinehelp.tableau.com/current/pro/desktop/en-us/embed_list.html)
