---
layout: post
title:  "Penny Exception Handler 0.0.1"
summary: "This library is an example of Exception Handler, in order to catch and render a readable exception, 
this library is an integration between penny and whoops"
author: Gianluca Arbezzano
author_url: https://twitter.com/gianarb
date:   2015-12-29 10:24:50
categories: community release
---
[Penny Exception Handler](https://github.com/pennyphp/excp-handler)  0.0.1 is ready!

* [[#1]](https://github.com/pennyphp/excp-handler/pull/1) make it works
* [[#4]](https://github.com/pennyphp/excp-handler/pull/4) Fixes #3 : Usage in readme in Skeleton App
* [[#6]](https://github.com/pennyphp/excp-handler/pull/6) Add travis conf

> whoops is an error handler base/framework for PHP. Out-of-the-box, it provides
> a pretty error interface that helps you debug your web projects, but at heart
> it's a simple yet powerful stacked error handling system.

This library provides an integration between Penny and
[whoops](https://github.com/filp/whoops). It uses into the [Penny Skeleton
Application](https://github.com/pennyphp/penny-skeleton-app) in order to render
readable errors.

This is the currenct integration into the Skeleton App

{% highlight php %}
<?php
return [
    'event_manager' => \DI\decorate(function($eventManager, $container) {
        $eventManager->attach("dispatch_error", [$container->get(WhoopsListener::class), "onError"]);
        $eventManager->attach("*_error", [$container->get(WhoopsListener::class), "onError"]);
        return $eventManager;
    }),
    WhoopsListener::class => \DI\object(WhoopsListener::class),
];
{% endhighlight %}

## Try
In order to understand how penny works you can try to
read this project and its tests, it contains [only one
class](https://github.com/pennyphp/excp-handler/blob/master/src/EventListener/WhoopsListener.php)!
