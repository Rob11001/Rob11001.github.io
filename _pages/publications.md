---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% if post.date %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

---

<h1>To be submitted:</h1>
{% for post in site.publications reversed %}
  {% if post.date %}
  {% else %}
    {% include archive-single-not-pub.html %}
  {% endif %}
{% endfor %}


