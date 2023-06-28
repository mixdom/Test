---
lng_pair: id_post_list
title: "Pastel Button"
author: Mixdom
category: code 
tags: [button, css, html]
img: ":Pastel_Button.png"
comments_disable: true
date: 2023-06-27 10:04:30 +0900
meta_modify_date: 2023-06-27 10:04:30 +0900
#meta_description: ""
image_viewer_on: true
image_lazy_loader_on: true
on_site_search_exclude: true
search_engine_exclude: true
#published: false
---

![Pastel Button](:Pastel_Button.png){:data-align="center"}

### Hover Effect with Pseudo-element

> **CSS**

```python
.cont {
  display: flex;
  align-items: center;
  justify-content: center
}

.slide {
  width: 150px;
  height: 40px;
  display: inline-block;
  font-size: 15px;
  line-height: 40px;
  text-align: center;
  letter-spacing: 5px;
  color: #FFF;
  background-color: #90E0F3;
  border-radius: 10px;
  overflow: hidden;
  transition: all .2s ease-in-out;
  text-transform: uppercase
}

.slide:hover {
  color: #FFF;
  background-color: #B8B3E9;
  transition: background-color 2s ease-out
}

.first, .second {
  padding-left: 5px;
  display: block;
  transition: all 420ms cubic-bezier(0.175, 0.885, 0.32, 1.275)
}

.slide:hover .first {
  margin-top: -38px
}

.box {
  width: 200px;
  height: 200px;
  background: #CCC
}

.box:hover {
  /*   background: linear-gradient(80deg, #90E0F3, #B8B3E9); */
  background-color: #B8B3E9;
  -webkit-transition: background-color 2s ease-out;
  -moz-transition: background-color 2s ease-out;
  -o-transition: background-color 2s ease-out;
  transition: background-color 2s ease-out
}
```

<br/>
> **HTML**

```python
<div class="cont">
<a href='#url' class="slide">
<div class="first">Download</div>
<div class="second">25MB</div>
</a>
</div>
```

<br/>
> **Result**

<style>
.cont {
  display: flex;
  align-items: center;
  justify-content: center
}

.slide {
  width: 150px;
  height: 40px;
  display: inline-block;
  font-size: 15px;
  line-height: 40px;
  text-align: center;
  letter-spacing: 5px;
  color: #FFF;
  background-color: #90E0F3;
  border-radius: 10px;
  overflow: hidden;
  transition: all .2s ease-in-out;
  text-transform: uppercase
}

.slide:hover {
  color: #FFF;
  background-color: #B8B3E9;
  transition: background-color 2s ease-out
}

.first, .second {
  padding-left: 5px;
  display: block;
  transition: all 420ms cubic-bezier(0.175, 0.885, 0.32, 1.275)
}

.slide:hover .first {
  margin-top: -38px
}

.box {
  width: 200px;
  height: 200px;
  background: #CCC
}

.box:hover {
  /*   background: linear-gradient(80deg, #90E0F3, #B8B3E9); */
  background-color: #B8B3E9;
  -webkit-transition: background-color 2s ease-out;
  -moz-transition: background-color 2s ease-out;
  -o-transition: background-color 2s ease-out;
  transition: background-color 2s ease-out
}
</style>

<div class="cont">
<a href='#url' class="slide">
<div class="first">Download</div>
<div class="second">25MB</div>
</a>
</div>
