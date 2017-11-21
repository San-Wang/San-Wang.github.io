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


>Embed code:  

~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=y&:display_count=yes"></iframe>
~~~  
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=y&:display_count=yes"></iframe>



>Code for adjusting dashboard size:    

~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=true" width = '600' height = '600'></iframe>
~~~  
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=true" width = '600' height = '600'></iframe>  



>Code to not show "Tableau Public" headline :  

~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true" width = '800' height = '800'></iframe>
~~~  
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true" width = '800' height = '800'></iframe>  


[Reference](http://kb.tableau.com/articles/howto/embedding-tableau-public-views-in-iframes)
