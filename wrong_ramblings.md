## Wrong Ramblings

It is just plain wrong.

{% assign wrong_ramblings = site.wrong_ramblings | sort: 'date' | reverse %}
{% include collection.md collection=wrong_ramblings %}
