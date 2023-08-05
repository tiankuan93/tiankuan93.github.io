---
permalink: /
title: "About me"
excerpt: "Research scientist at Tencent AI Lab."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

This is Tian Kuan's home on the web!

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
