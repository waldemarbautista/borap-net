---
layout: default
---

{% assign collection = site.collections | where: 'label', page.collection | first %}

{% capture md %}

## {{ collection.title }}
{{ collection.description }}

* * *
### {{ page.title }}
{{ content }}

{% endcapture %}
{{ md | markdownify }}
