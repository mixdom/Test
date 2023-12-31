---
lng_pair: id_post_list
title: "CSS Pulsing Button"
author: Mixdom
category: code 
tags: [button, css, html]
img: ":CSS_Pulsing_Button.png"
comments_disable: false
date: 2023-06-27 10:04:30 +0900
meta_modify_date: 2023-06-27 10:04:30 +0900
meta_description: "Tutorial Blog: Cara Membuat CSS Pulsing Button"
image_viewer_on: true
image_lazy_loader_on: true
#on_site_search_exclude: true
#search_engine_exclude: true
#published: false
---

![CSS Pulsing Button](:CSS_Pulsing_Button.png){:data-align="center"}

***

> **CSS**

```python
.bg,
.oibutton {
  position: absolute;
  width: 50px;
  height: 50px;
  border-radius: 100%
}

.cont {
  display: flex;
  align-items: center;
  justify-content: center
}

.bg {
  animation: pulse 1.2s ease infinite;
  background: #ff3466
}

.oibutton {
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  z-index: 99;
  border: none;
  background: #ff3466;
  background-size: 18px;
  cursor: pointer;
  outline: none
}

.oibutton a {
  position: absolute;
  color: #FFF;
  font-size: 17px
}

@keyframes pulse {
  0% {
    transform: scale(1, 1)
  }
  50% {
    opacity: 0.3
  }
  100% {
    transform: scale(1.5);
    opacity: 0
  }
}
```

<br/>
> **HTML**

```python
<div class="cont">
<div class="bg">
</div>
<div class="oibutton">
<a href="#url"><i class="fa fa-chevron-down" aria-hidden="true"></i></a>
</div>
</div>
```

<br/>
> **Result**

<style>
.bg,
.oibutton {
  position: absolute;
  width: 50px;
  height: 50px;
  border-radius: 100%
}

.cont {
  display: flex;
  align-items: center;
  justify-content: center
}

.bg {
  animation: pulse 1.2s ease infinite;
  background: #ff3466
}

.oibutton {
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  z-index: 99;
  border: none;
  background: #ff3466;
  background-size: 18px;
  cursor: pointer;
  outline: none
}

.oibutton a {
  position: absolute;
  color: #FFF;
  font-size: 17px
}

@keyframes pulse {
  0% {
    transform: scale(1, 1)
  }
  50% {
    opacity: 0.3
  }
  100% {
    transform: scale(1.5);
    opacity: 0
  }
}
</style>

<br/>

<div class="cont">
<div class="bg">
</div>
<div class="oibutton">
<a href="#url"><i class="fa fa-chevron-down" aria-hidden="true"></i></a>
</div>
</div>

<br/>

<br/>
