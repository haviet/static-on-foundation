---
layout: default
title: Liên hệ
tags: topnav
permalink: contact/
w: 4
---

<div class="row show-for-medium-up">
	<div class="columns">
		<p><img src="http://placehold.it/1150x500&text=insert+google+maps" /></p>
		<p>Ban co the lien he voi cac phong chuc nang bang cac so dien thoai duoc cung cap duoi day. Hoac <a href="#" data-reveal-id="directmail" class="alert label round">gui email truc tiep</a> cho chung toi.</p>
	
		<div id="directmail" class="reveal-modal large" data-reveal>
			{% include lienhe.html %}
		</div>

	</div>
</div>

<div class="row">
	<div class="columns">
		<br>
		<div class="panel callout text-centered">
			<h4>Haviet luon san sang lang nghe moi y kien dong gop cua khach hang.</h4>
		</div>
	</div>
</div>

<div class="row show-for-medium-up"> <!-- hiển thị trên màn hình lớn -->
	<div class="columns">
		<ul class="medium-block-grid-3">
		{% for contact in site.data.contacts %}
			<li>
				<img src="{{ contact.imagelink }}" />
				<h5>{{ contact.name }}</h5>
				<p>{{ contact.desc }}</p>
				<p class="contact-line">
					<span><img src="{{ site.baseurl }}/{{ site.imgs }}/icon-phone.svg" width="16px" /></span> {{ contact.tel }}<br>
					<span><img src="{{ site.baseurl }}/{{ site.imgs }}/icon-email.svg" width="16px" /></span> {{ contact.email }}
				</p>
			</li>
		
		{% endfor %}
		</ul>
	</div>
</div>

<div class="row show-for-small-only"> <!-- hiển thị trên màn hình nhỏ -->
	<div class="columns">
		<ul class="no-bullet text-centered">
		{% for contact in site.data.contacts %}
			<li>
				<h5>{{ contact.name }}</h5>
				<p class="contact-line">
					<span>Tel: {{ contact.tel }}<br>
					<span>Email: {{ contact.email }}
				</p>
			</li>
		
		{% endfor %}
		</ul>
	</div>
</div>
