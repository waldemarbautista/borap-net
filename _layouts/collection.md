---
layout: default
---

{{ content }}

{% assign collection = site.collections | where: 'label', page.collection | first %}
{% assign collection = collection.docs | sort: 'date' | reverse %}

{% capture md %}

{% for item in collection %}
* * *
### {{ item.title }}
{{ item.excerpt }}
[Read more]({{ item.url }})
{% endfor %}

{% endcapture %}
{{ md | markdownify }}
