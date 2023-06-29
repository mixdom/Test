---
lng_pair: id_post_list
title: "Animated Gradient Button (Pure CSS)"
author: Mixdom
category: code 
tags: [button, css, html]
img: ":Animated_Gradient_Button-Pure_CSS.png"
comments_disable: false
date: 2023-06-29 10:05:30 +0900
meta_modify_date: 2023-06-29 10:05:30 +0900
meta_description: "Tutorial Blog: Cara Membuat Animated Gradient Button (Pure CSS)"
image_viewer_on: true
image_lazy_loader_on: true
#on_site_search_exclude: true
#search_engine_exclude: true
#published: false
---

![Pastel Button](:Animated_Gradient_Button-Pure_CSS.png){:data-align="center"}

***

> **CSS**

```python
.body {
  display: flex;
  align-items: center;
  justify-content: center
}
.btn,
.btn2 {
  width: 300px;
  height: 100px;
  font-size: 30px;
  text-align: center;
  line-height: 100px;
  color: rgba(255,255,255,0.9);
  border-radius: 50px;
  background: linear-gradient(-45deg, #ffa63d, #ff3d77, #338aff, #3cf0c5);
  background-size: 600%;
  -webkit-animation: anime 16s linear infinite;
          animation: anime 16s linear infinite
}
.btn2 {
  position: absolute;
  margin-top: -70px;
  z-index: -1;
  -webkit-filter: blur(30px);
          filter: blur(30px);
  opacity: 0.8
}
@-webkit-keyframes anime {
  0% {
    background-position: 0% 50%
  }
  50% {
    background-position: 100% 50%
  }
  100% {
    background-position: 0% 50%
  }
}
@keyframes anime {
  0% {
    background-position: 0% 50%
  }
  50% {
    background-position: 100% 50%
  }
  100% {
    background-position: 0% 50%
  }
}
```

<br/>
> **HTML**

```python
<div class='body'>
<a href='#url'>
<div class="btn">
Gradient Button
<div class="btn2">
</div>
</div>
</a>
</div>
```

<br/>
> **Result**

<style>
.body {
  display: flex;
  align-items: center;
  justify-content: center
}
.btn,
.btn2 {
  width: 300px;
  height: 100px;
  font-size: 30px;
  text-align: center;
  line-height: 100px;
  color: rgba(255,255,255,0.9);
  border-radius: 50px;
  background: linear-gradient(-45deg, #ffa63d, #ff3d77, #338aff, #3cf0c5);
  background-size: 600%;
  -webkit-animation: anime 16s linear infinite;
          animation: anime 16s linear infinite
}
.btn2 {
  position: absolute;
  margin-top: -70px;
  z-index: -1;
  -webkit-filter: blur(30px);
          filter: blur(30px);
  opacity: 0.8
}
@-webkit-keyframes anime {
  0% {
    background-position: 0% 50%
  }
  50% {
    background-position: 100% 50%
  }
  100% {
    background-position: 0% 50%
  }
}
@keyframes anime {
  0% {
    background-position: 0% 50%
  }
  50% {
    background-position: 100% 50%
  }
  100% {
    background-position: 0% 50%
  }
  }
</style>

<div class='body'>
<a href='#url'>
<div class="btn">
Gradient Button
<div class="btn2">
</div>
</div>
</a>
</div>
