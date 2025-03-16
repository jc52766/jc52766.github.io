---
title: "Jarmonica"
categories: [Harmonica, J, Music]
tags: [Harmonica, J, Music]
---

# Jarmonica - Generating harmonica exercises with J
<br/>
As a beginner harmonica player I need fresh exercises.<br/>
Exercises to improve single note playing and accuracy jumping holes.<br/>
<br/>
```j
{% raw %}
   pos=:1 NB. position? 1st, 2nd, ...
   xi=:4 NB. which notes to pick from per pattern? 2,3,4,...?
   ]xo=:(- , ]) pos+i.xi NB. options
_1 _2 _3 _4 1 2 3 4
   xnn=:4 NB. how many notes per patterns?
   rs=: 3 : '?#xo'
   xnp=:10 NB. how many patterns to randomly select?
   xs=:{{< xo {~ rs"0] i.xnn}}"0 i.xnp
   >xs
 4 _2 _1 _2
_1 _1  4  1
 3  4 _3 _4
_3  1 _1 _2
_1 _2  1 _4
_3  1  3 _1
 2  4 _3  4
 2  1  3  1
_4  4 _1 _2
 2 _1  4 _1
   
 {% endraw %}
 ```
<br/>
