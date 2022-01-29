---
layout: default
---

# Posts:

{% for post in site.posts %}
* ## [{{ post.title }}]({{ post.url }})
###### {{ page.date | date: "%-d %B %Y" }} by {{ post.author}}
###### Tags: {% for tag in post.tags %} {{tag}}, {% endfor %}

{% endfor %}