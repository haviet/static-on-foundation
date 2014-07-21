---
layout: default
title: Khách hàng - Đối tác
tags: topnav
permalink: clients/
w: 3
---

<div class="row show-for-medium-up"> <!-- chi hien thi tren man hinh lon -->
	<div class="columns">
		<img src="http://placehold.it/1150x250" />
	</div>
</div>


<div class="row">
	<br>
	<div class="columns">
		{% include khdt-content.html %}
	</div>
</div>

<div class="row">
	<div class="columns">
		<br>
		<div class="panel callout text-centered">
			<h4>Hop tac luon la phuong cham dan dau moi hoat dong cua chung toi.</h4>
		</div>
	</div>
</div>

<!-- hien thi tren man hinh lon -->
<div class="row show-for-medium-up">
	<div class="columns">
		<ul class="home-slideshow" data-orbit>
	    	{% for slideshow in site.data.home-slideshow %}
		    <li>
		    	<img src="{{ site.baseurl }}/{{ slideshow.link }}" alt="{{ slideshow.alt }}" />
		    	<div class="orbit-caption">{{ slideshow.caption }}</div>
		    </li>
	    	{% endfor %}
	  	</ul>
	</div>
</div>

<!-- hien thi tren man hinh nho -->
<div class="row show-for-small-only">
	<div class="columns">
		<img src="http://placehold.it/640x400" />
	</div>
</div>