---
layout: default
title: RRIS
---
{% for r in site.data.myrepos %}
# {{  r.name }}
{% endfor %}
{% highlight ruby %}
def foo
  puts 'foo'
end
{% endhighlight %}
