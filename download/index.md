---
layout: default
title: Downloads
---

Get the good stuff here.


<ul>
{% for version in site.data.downloads %}
  <li>
    {{ version.name }}
    <ul>
		{% for dl in version.platforms %}
  		<li><a href="{{ dl.urlroot }}">{{ dl.platform }}</a></li>
		{% endfor %}
	</ul>
  </li>
{% endfor %}
</ul>

