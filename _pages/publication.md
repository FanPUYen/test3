---
layout: archive
title: "Publication List"
permalink: /publication/
author_profile: true
---

{% include base_path %}

{% assign pubs = site.publications | sort: 'date' | reverse %}

### Journal Articles
{% for pub in pubs %}
{% if pub.category == 'manuscripts' %}
- {{ pub.title }} ({{ pub.date | date: '%Y' }})
{% endif %}
{% endfor %}

### Conference Papers
{% for pub in pubs %}
{% if pub.category == 'conferences' %}
- {{ pub.title }} ({{ pub.date | date: '%Y' }})
{% endif %}
{% endfor %}

### Books
{% for pub in pubs %}
{% if pub.category == 'books' %}
- {{ pub.title }} ({{ pub.date | date: '%Y' }})
{% endif %}
{% endfor %}
