---
layout: page
title: Archive
permalink: /archive/
subtitle: "The List"
imgurl: /img/contact-bg.jpg
---

<div class="container">
    <div class="row">
        <div class="col-lg-8 col-lg-offset-2 col-md-10 col-md-offset-1">
        	<ul>
				{% for post in site.posts %}
					<li>{{ post.date | date_to_string }} &raquo; <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></li>
				{% endfor %}
			</ul>
		</div>
	</div>
</div>