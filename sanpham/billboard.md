---
layout: default
title: Biển quảng cáo tấm lớn
tags: hotprd
permalink: haviet-billboard/
---

<div class="row">
  <div class="columns">
  <p class="panel callout lead">Biển tấm lớn - Billboard</p>
  
  <h2>Available</h2>

<table style="width:100%;">
  <thead>
    <tr> 
      <th>Codename</th>
      <th>Location</th> 
      <th>Describe</th>
      <th>Size</th>
    </tr>
  </thead>
  <tbody> 
  {% for post in site.categories.billboard %}
  {% if post.available == true %}
    <tr>
      <td><a href="{{ post.url }}">{{ post.codename }}</a></td>
      <td>{{ post.location }}</td>
      <td>{{ post.desc }}</td>
      <td>{{ post.size }}</td>
    </tr>
  {% endif %}
  {% endfor %}
  </tbody>
</table> 
  
  
  <h2>Rented</h2>
<table style="width:100%;">
  <thead>
    <tr> 
      <th>Codename</th>
      <th>Describe</th>
      <th>Size</th>
      <th>Due Date</th> 
    </tr>
  </thead>
  <tbody> 
  {% for post in site.categories.billboard %}
  {% if post.available == false %}
    <tr>
      <td><a href="{{ post.url }}">{{ post.codename }}</a></td>
      <td>{{ post.desc }}</td>
      <td>{{ post.size }}</td>
      <td>{{ post.duedate }}</td>
    </tr>
  {% endif %}
  {% endfor %}
  </tbody>
</table> 
  
  
  
  
    
  </div>
</div>


<!-- hiển thị trên màn hình lớn -->
<div class="row show-for-medium-up">
  <div class="columns">
     <h4>Các sản phẩm khác</h4>
  	{% include sp-bigblock-list.html %}
  </div>
</div>

<!-- hiển thị trên màn hình nhỏ -->
<div class="row show-for-small-only">
	<div class="columns">
		<h4>Các sản phẩm khác</h4>
		{% include sp-list.html %}
	</div>
</div>
