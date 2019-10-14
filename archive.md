---
layout: page
title: Blog archive
---
<div class="page-content wc-container">
  {% for post in site.posts %}
  	{% capture currentyear %}{{post.date | date: "%Y"}}{% endcapture %}
  	{% if currentyear != year %}
    	{% unless forloop.first %}</ul>{% endunless %}
    		<h5>{{ currentyear }}</h5>
    		<ul class="posts">
    		{% capture year %}{{currentyear}}{% endcapture %}
  		{% endif %}
    <li><span>{{ post.date | date: "%B %-d"}} - <a href="{{ post.url }}">{{ post.title }}</a></span></li>
    {% if forloop.last %}</ul>{% endif %}
{% endfor %}
</div>
