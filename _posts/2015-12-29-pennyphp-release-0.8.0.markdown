---
layout: post
title:  "Penny 0.8.0, the last release of 2015"
summary: "Penny is a middleware PHP framework made to increase interoperability
between PHP libraries, this post contains changelog of release 0.8.0"
author: Gianluca Arbezzano
author_url: https://twitter.com/gianarb
date:   2015-12-29 10:24:50
categories: core release
---
Penny PHP Framework 0.8.0 is ready!

* [[#145]](https://github.com/pennyphp/penny/pull/145) make bootstrap event triggered in App::run()
* [[#147]](https://github.com/pennyphp/penny/pull/147) Fixes [[#96]](https://github.com/pennyphp/penny/pull/96) , implements ClassName::class prefix for event name
* [[#150]](https://github.com/pennyphp/penny/pull/150) update symfony/http-foundation to ~3.0
* [[#151]](https://github.com/pennyphp/penny/pull/151) remove php7 from allow_failures in travis config
* [[#146]](https://github.com/pennyphp/penny/pull/146) remove ->getContainer() call inside internal App class inside setUpEventWithRequestResponse() method
* [[#152]](https://github.com/pennyphp/penny/pull/152) add exception message to RouteNoutFoundException and MethodNotAllowedException
* [[#154]](https://github.com/pennyphp/penny/pull/154) Add test dispatcher is a closure
* [[#155]](https://github.com/pennyphp/penny/pull/155) Fixed Readme.md and add site

## BC Break

1. Our app new triggers

{% highlight php %}
$eventManager->attach(App\Controller\IndexController::class.".index", ...)
{% endhighlight %}
Because in our opinion this method is more readable and easy to maintain.

[Github Milestone](https://github.com/pennyphp/penny/releases/tag/0.8.0)
