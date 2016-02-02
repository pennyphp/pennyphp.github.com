---
layout: post
title:  "Penny expception handler 0.0.2 is ready to go"
summary: "Penny is a middleware PHP framework made to increase interoperability
between PHP libraries, this library manages integration with whoops to print pretty our excpetions"
author: Gianluca Arbezzano
author_url: https://twitter.com/gianarb
date:   2015-12-29 10:24:50
categories: core release
---
[Penny Excpetion Handler](https://github.com/pennyphp/excp-handler) 0.0.2 is ready!

We have fixed whoops's version, now we require `^1.0`.

If somebody has time and experience we are very happy to update our library to
work with the whoops 2.0.

Remember to change your composer.json

{% highlight json %}
{
    "penny/excp-handler": "0.0.2"
}
{% endhighlight %}

See [this article](http://pennyphp.org/blog/penny-excp-handler-0.0.1/) to understand how it works

[Github Milestone](https://github.com/pennyphp/excp-handler/releases/tag/0.0.2)
