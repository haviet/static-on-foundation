---
layout: default
title: Giới thiệu
tags: topnav
permalink: intro/
w: 1
---

<!-- top page image, can be slideshow depend on requirement -->
<div class="row">
	<div class="columns show-for-medium-up">
		<img src="{{ site.baseurl }}/{{ site.imgs }}/advertising-banner.jpg" />
	</div>
	<div class="columns show-for-small-only">
		<img src="http://placehold.it/640x400" />
	</div>
</div>

<div class="row">
	<br>
	<div class="columns">
		<div class="panel callout text-centered">
			<h4>Cong ty Haviet khong ngung tim kiem co hoi hop tac</h4>
		</div>
	</div>
</div>

<!-- hiển thị trên màn hình lớn -->
<div class="row show-for-medium-up clearfix">
	<div class="medium-8 columns">
		<h3>Giới thiệu chung</h3>
		<p>nội dung giới thiệu chi tiết về công ty</p>
		<p><img src="http://placehold.it/640x400" /></p>
		<h3>Lịch sử phát triển</h3>
		<p>Các giai đoạn phát triển của công ty</p>
		<h3>Hoạt động đầu tư</h3>
		<p>Danh sách các hoạt động đầu tư tiêu biểu</p>
		<p><img src="http://placehold.it/640x480" /></p>
	</div>
	<div class="medium-4 columns">
	<h3>Sản phẩm tiêu biểu</h3>
		<ul class="no-bullet">
			{% for link in site.data.link-bigblock %}
		  	<li>
		  		<a href="{{ site.baseurl }}/{{ link.linkto }}">
		  			<div>
		  				<p><img src="{{ link.image }}" /></p>
		  				<p>{{ link.name }}</p>
		  			</div>
		  		</a>
		  	</li>
			{% endfor %}
		</ul>		
	</div>
</div>

<!-- hiển thị trên màn hình nhỏ -->
<div class="row show-for-small-only">
	<div class="columns">
		<h3>Giới thiệu chung</h3>
		<p>Nội dung phần giới thiệu chung</p>
		<p><img src="http://placehold.it/640x400" /></p>
		<h3>Sản phẩm tiêu biểu</h3>
		<ul>
			{% for link in site.data.link-bigblock %}
				<li><a href="{{ site.baseurl }}/{{ link.linkto }}">{{ link.name }}</a></li>
			{% endfor %}
		</ul>
	</div>
</div>
