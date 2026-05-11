+++
date = '2026-04-10T14:03:27+02:00'
draft = false
title = '♾️ Geogebra'
tags = ['capes', 'maths']
+++

# Suite récurrente

- définir f: 
- definir un u0:
- définir la suite u  
- définir la liste des points Un sur l'axe des abscisses
- définir les projections des  Un sur l'axe y=x 
- définir les projections des  Un sur  y=f(x) 
- définir les segments verticaux 
- définir les segments horizontaux

```
f:=sqrt(x)
uO=1
u:= IterationList(f, u0, 10)
P = Sequence((Element(u, k), 0), k, 0, Length(u) - 1)
Q = Sequence((Element(u, k), Element(u, k)), k, 0, Length(u) - 1)
hor:= Sequence(Segment((Element(u, k), f(Element(u, k))), (f(Element(u, k)), f(Element(u, k)))), k, 0, Length(u) - 2)
vert:= Sequence(Segment((Element(u, k), Element(u, k)), (Element(u, k), f(Element(u, k)))), k, 0, Length(u) - 2)
```
