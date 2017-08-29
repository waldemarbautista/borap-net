{% for item in include.collection %}
* * *
### {{ item.title }}
{{ item.content }}
{% endfor %}
