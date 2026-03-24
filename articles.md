---
layout: default
title: Articles
---

# Articles
This page is organized as a tree:
**Topic -> Year -> Post**

[How to add a new article](/POSTING_GUIDE.md)

{% assign sorted_categories = site.categories | sort %}
{% if sorted_categories.size > 0 %}
{% for category in sorted_categories %}
## {{ category[0] | capitalize }}
{% assign posts_by_year = category[1] | group_by_exp: "post", "post.date | date: '%Y'" %}
{% for year in posts_by_year %}
### {{ year.name }}
{% for post in year.items %}
* [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%b %d" }}
{% endfor %}
{% endfor %}
{% endfor %}
{% else %}
No posts yet.
{% endif %}
