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


Embed code:  
~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=y&:display_count=yes"></iframe>
~~~
  
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:embed=y&:display_count=yes"></iframe>


Embed code to show dashboard without :  
~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true"></iframe>
~~~
  
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true"></iframe>


Embed code for adjusting dashboard size:    
~~~ ruby
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true" width = '1000' height = '800'></iframe>
~~~  
<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true" width = '1000' height = '800'></iframe>  

~~~ ruby
<script>
  function resizeIframe(obj) {
    obj.style.height = obj.contentWindow.document.body.scrollHeight + 'px';
  }
</script>

<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true" frameborder="0" scrolling="no" onload="resizeIframe(this)" />
~~~  

<script>
  function resizeIframe(obj) {
    obj.style.height = obj.contentWindow.document.body.scrollHeight + 'px';
  }
</script>

<iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true" frameborder="0" scrolling="no" onload="resizeIframe(this)" />

~~~ ruby
<div class="intrinsic-container intrinsic-container-16x9">
  <iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true" allowfullscreen></iframe>
</div>

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
~~~  

<div class="intrinsic-container intrinsic-container-16x9">
  <iframe src="https://public.tableau.com/views/GTSRB_Result_Viz/GTSRB?:showVizHome=no&:embed=true" allowfullscreen></iframe>
</div>

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

[Reference](http://kb.tableau.com/articles/howto/embedding-tableau-public-views-in-iframes)
