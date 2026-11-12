---
layout: page
title: Letters
permalink: /letters/
---

*Letters Marikai wrote to her future self.*

{% assign entries = site.letters | sort: "written_on" | reverse %}

{% for entry in entries %}
- Written {{ entry.written_on }}{% if entry.time %} at {{ entry.time }}{% endif %} — [read]({{ entry.url | prepend: site.baseurl }})
{% endfor %}
