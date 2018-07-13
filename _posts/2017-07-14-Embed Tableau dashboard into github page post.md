---
layout: post
title: Embed Tableau dashboard into github page post
excerpt: "Visualization - Tableau"
modified: 10/23/2017
tags: [Visualization, Tableau]
comments: true
category: blog
---  

After spending a lot of time searching online on how to embed tableau dashboard into my blog, I figure it would save people who want to do the same thing as me some time if I post my finding here. I will put the code I tried with the result that the dashboard showed in my blog together. 

I am still exploring the best way to embed tableau that can automatically adjust dashboard size along with content.


>Basic embed code:  
Works fine on a regular whole page size website, but not suitable for my github page website.

~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=yes&:display_count=yes"></iframe>
~~~  
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=yes&:display_count=yes"></iframe>



>Code for adjusting dashboard size:    

~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=yes&:display_count=yes" width = '600' height = '600'></iframe>
~~~   
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=yes&:display_count=yes" width = '600' height = '600'></iframe>  



>Code to not show "Tableau Public" headline :  

~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=yes&:display_count=yes" width = '650' height = '800'></iframe>
~~~  
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=yes&:display_count=yes" width = '650' height = '800'></iframe>  


>Get rid of border:

~~~ ruby
<iframe seamless frameborder="0" src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=yes&:display_count=yes" width = '650' height = '800'></iframe>  
~~~  
<iframe seamless frameborder="0" src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=yes&:display_count=yes" width = '650' height = '800'></iframe>  


>Next step: automatically adjust tableau dashboard to make it fit within the iframe  
Caution: Enable to use auto scale, need to set dashboard size as auto in Tableau Desktop!

~~~ ruby
<iframe seamless frameborder="0" src="https://public.tableau.com/views/GTSRB_Viz/GTSRB?:showVizHome=no&:embed=yes&:display_count=yes" width = '650' height = '450' scrolling='yes' ></iframe>    
~~~  

<iframe seamless frameborder="0" src="https://public.tableau.com/views/GTSRB_Viz/GTSRB?:showVizHome=no&:embed=yes&:display_count=yes" width = '650' height = '450' scrolling='yes' ></iframe>    


_________________________
[Reference](http://kb.tableau.com/articles/howto/embedding-tableau-public-views-in-iframes)  
[Parameters for Embed Code](https://onlinehelp.tableau.com/current/pro/desktop/en-us/embed_list.html)
