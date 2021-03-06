---
title: Rotate
description: Rotate a view.
date:   2016-05-26 00:13:00 -0700
layout: example
categories: examples, views
permalink: /examples/views-rotate/
image: poster.png
tags: [views, transform, rotate]
author: Travis Kirton
---
![](rotate.png)

## Rotate
You can rotate a view by creating a `Transform` and setting it to the view's property:

{% highlight swift lineos %}
view.transform = Transform.makeRotation()
{% endhighlight %}

> Rotating a Transform will adjust itself between `-M_PI` and `M_PI`, if you need to accumulate or set rotations higher than `+/- PI` you can use the `.rotation` property.

## Example
{% highlight swift lineos %}
let r = Rectangle(frame: Rect(0, 0, 200, 200))
r.lineWidth = 15.0
r.center = canvas.center

let rotate = Transform.makeRotation(M_PI_4)
r.transform = rotate

canvas.add(r)
{% endhighlight %}
