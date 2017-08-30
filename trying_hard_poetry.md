## Trying Hard Poetry

At least, trying hard.

{% assign trying_hard_poetry = site.trying_hard_poetry | sort: 'date' | reverse %}
{% include collection.md collection=trying_hard_poetry %}
