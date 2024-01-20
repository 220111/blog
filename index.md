---
layout: default
---

# Posts

{% for post in site.posts %}
<div>
    <hr>
    <h2><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
    <img src="{{post.image | prepend: site.baseurl}}" style="max-width:50%">
    <p>{{post.excerpt}}</p>
</div>
{% endfor %}
