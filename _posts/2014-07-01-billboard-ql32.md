---
layout: post
codename: QL32
categories: billboard
location: Từ Liêm
desc: Gần trường ĐH Công nghiệp Hà Nội
nface: 2
size: 8m x 5m
available: no
duedate: 7/2015
images:
  - preview:
      http://placehold.it/380x350
      http://placehold.it/380x350
      http://placehold.it/380x350
  - full:
      http://placehold.it/1150x900
      http://placehold.it/1150x900
      http://placehold.it/1150x900
---

biển quốc lộ 32, trạm trung chuyển nhổn.

<ul>
{% for img in post.images %}
<li><a href="{{ img.full }}"><img src="{{ img.preview }} /></li>
{% endfor %}
</ul>