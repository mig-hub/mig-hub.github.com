---
layout: main
title: Mig Hub
---

Hello World
===========

This is a test.

    $ mkdir gogo
    $ cd gogo

{% highlight ruby %}
def my_method(name)
  puts "Hello #{name}"
end
{% endhighlight %}

{% for post in site.posts limit:5 %}
<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
{{ post.content }}
<em>Posted on {{ post.date | date_to_long_string }}.</em>
{% endfor %}