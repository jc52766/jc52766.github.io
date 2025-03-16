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
  'pos xi xnn xnp'=:1;4;6;5 NB. pos, n notes, n notes per pattern,  how many patterns?
   xo=:(- , ]) pos+i.xi
   rs=: 3 : '?#xo'
   xs=:{{< xo {~ rs"0] i.xnn}}"0 i.xnp
   >xs
 2 _4 _2 _4 _1  1
_3  1  1 _3  4 _3
 2 _4 _1 _3 _1  2
 2 _4  2 _3  1 _1
_2  1  1 _3 _4 _3
 {% endraw %}
 ```
<br/>
