---
title: Animating a Gradient
description: You can animate all the properties of a gradient.
date:   2016-05-06 23:59:59 -0800
layout: example
categories: examples
permalink: /examples/gradients-animate/
image: poster.png
tags: [getting started, basics, introduction, easy, c4]
author: Travis Kirton
---
![](animate.png)

## Animating a Gradient
Check out this mind-blowing example of how to animate a gradient.

## Example
{% highlight swift lineos %}
let g = Gradient(frame: canvas.frame)
canvas.add(g)

let a = ViewAnimation(duration: 1.0) {
    g.colors = [C4Purple, C4Grey]
    g.startPoint = Point(1, 0)
    g.endPoint = Point(0, 1)
    g.locations = [0.49, 0.51]
}

a.delay = 1.0
a.autoreverses = true
a.repeats = true
a.animate()
{% endhighlight %}