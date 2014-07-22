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
- preview: 380x250
  full: 1000x600
  caption: this is image one
- preview: 380x250
  full: 1000x600
  caption: this is image one
- preview: 380x250
  full: 1000x600
  caption: this is image one


---

biển quốc lộ 32, trạm trung chuyển nhổn.

<ul class="clearing-thumbs medium-block-grid-3" data-clearing>
{% for img in page.images %}
  <li><a href="http://placehold.it/{{ img.full }}"><img data-caption="{{ img.caption }}" src="http://placehold.it/{{ img.preview }}"></a></li>
{% endfor %}
</ul>