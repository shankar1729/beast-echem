---
layout: page
title: News
description: "Latest developments in the BEAST collaboration"
permalink: /news/
---

# News

{% for post in site.posts %}                                                                                                                                                                                  
+ {{ post.date | date: "%b %-d, %Y" }}: [ {{ post.title }} ]( {{ post.url | prepend: site.baseurl }} )
{% endfor %}
