---
title: Gradient Fill
description: Fill your shapes with gradients.
date:   2016-05-10 05:59:59 -0800
layout: example
categories: examples
permalink: /examples/shapes-gradient-fill/
image: poster.png
tags: [getting started, basics, introduction, easy, c4]
author: Travis Kirton
---
![](gradient-fill.png)

## Gradient Fills
Oh yes. Yes... Yes, you can fill your shapes with gradients.

## Example
{% highlight swift lineos %}
let star = Star(center: canvas.center, pointCount: 30, innerRadius: 125, outerRadius: 150)
star.gradientFill = Gradient(frame: star.bounds)
canvas.add(star)
{% endhighlight %}