---
layout: post
title: Embed Tableau dashboard into github page post
excerpt: "Visualization - Tableau"
modified: 10/23/2017
tags: [Visualization, Tableau]
comments: true
category: blog
---  

Here are some note for myself to embed tableau dashboard into blog after trying several different ways.

Embed code:  
~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true"
~~~
Outcome:  
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true"

Embed code for adjusting dashboard size:    
~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true" width = '800' height = '600'></iframe>
~~~  
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true" width = '800' height = '600'></iframe>



[Reference](http://kb.tableau.com/articles/howto/embedding-tableau-public-views-in-iframes)
