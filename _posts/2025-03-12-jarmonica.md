---
title: "Jarmonica"
categories: [Harmonica, J, Music]
tags: [Harmonica, J, Music]
---

# Jarmonica - Generating harmonica exercises with J
<br/>
J strikes again. With such an easy solution to the problem.<br/>
<br/>
As a beginner harmonica player I wanted fresh exercises.<br/>
I also didn't want to be limited by my own imagination and non-randomness.<br/>
I needed exercises that get me used to playing different single notes across randomly selected holes.<br/>
<br/>
```j
pos=:1 NB. position? 1st, 2nd, ...
xi=:4 NB. which notes to pick from per pattern? 2,3,4,...?
]xo=:(- , ]) pos+i.xi NB. options
xnn=:4 NB. how many notes per patterns?
rs=: 3 : '?#xo'
xnp=:10 NB. how many patterns to randomly select?
]xs=:{{< xo {~ rs"0] i.xnn}}"0 i.xnp
,.>,.xs
 2 _3  3  3
 4  1 _4 _2
_3 _1  2  4
_2 _4  3 _4
_4  2 _1  4
_1 _2  1  2
_4  4 _3 _1
_3  4  3 _1
 1  4 _3  1
 1  2  4  2
 ```
<br/>
