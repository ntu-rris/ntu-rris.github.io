---
layout: default
title: RRIS home
---
{% for r in site.data.myrepos %}
[{{ r.name }}]({{r.html_url|absolute_url}})
<br/>**{{ r.description| default: "No Description" }}**
  <br/> contributors: {% for j in r.contrib %} [{{j.login}}]({{j.html_url|absolute_url}}) {% endfor %}
{% endfor %}
