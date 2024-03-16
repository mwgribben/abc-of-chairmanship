{% for item in site.data.contents.pages %}
- [{{ item.title }}]({{ item.url }})
{% endfor %}
