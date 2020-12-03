---
layout: default
---

# Posts:

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})
Author: {{ post.author}}

Date: {{ post.date}}

Category: {{ post.category }}

Tags: {{ post.tags }}

{% endfor %}