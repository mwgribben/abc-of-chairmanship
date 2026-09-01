---
last_modified_at: 2023-01-02
canonical_url: 'https://chair.guide'
title: ABC of Chairing
---

# Contents

## Front matter

{% for item in site.data.contents.pages limit: 3 %}
- [{{ item.title }}]({{ item.url }})
{% endfor %}

## Chapters

{% for item in site.data.contents.pages offset: 3 limit: 14 %}
- [{{ item.title }}]({{ item.url }})
{% endfor %}

## Appendices

{% for item in site.data.contents.pages offset: 17 %}
- [{{ item.title }}]({{ item.url }})
{% endfor %}
