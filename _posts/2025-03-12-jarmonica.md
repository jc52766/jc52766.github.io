---
title: "Jarmonica"
categories: [Harmonica, J, Music]
tags: [Harmonica, J, Music]
---

# Jarmonica - Generating harmonica exercises with J
<br/>
<br/>
```j
{% raw %}  'pos xn xnpp xnp'=:1;4;6;5 NB. pos, n notes, n notes per pattern, how many patterns
   xo=:(- , ]) pos+i.xn
   rs=: 3 : '?#xo'
   xs=:{{< xo {~ rs"0] i.xnpp}}"0 i.xnp
   >xs
 1 _3  4 _1 _4 _3
_1  1 _3  4 _3 _4
 2  3  3 _4  1 _2
 2 _2  2  4 _4  1
 4  4  2  4 _4  4{% endraw %}
 ```
<br/>
