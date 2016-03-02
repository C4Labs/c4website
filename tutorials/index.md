---
layout: page
title: 'Basics'
categories: cosmos, tutorials
---

## Tutorials

<div class="row">
	<div class="col-xs-12 col-md-12">
		<ul class="examples-list list-unstyled">
			{% assign tutorialsPosts = site.categories['tutorials'] | sort: 'order' %}
			{% for post in tutorialsPosts %}
			  <li>
			  	<a href="{{ post.url }}">
			  		<div>
			  			<span class="img">
				  			<img src="{{ site.baseurl }}/images/cosmos/{{ post.chapter }}/{{ post.image }}" />
				  		</span>
				  		<div class="text">
					  		<p class="title">{{ post.title }}</p>
					  		<p>{{ post.description }}</p>
					  	</text>
				  	</div>
				  </a>
			  </li>
			{% endfor %}
		</ul>
	</div>
</div>