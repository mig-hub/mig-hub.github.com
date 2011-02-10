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
[{{ post.title }}]({{ post.url }})
_Posted on {{ post.date | date_to_long_string }}._
{% endfor %}