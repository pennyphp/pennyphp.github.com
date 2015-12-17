---
layout: post
title:  "Penny 0.7.0, good morning"
summary: "Penny is a middleware PHP framework made to increase interoperability
between PHP libraries, this post contains changelog of release 0.5.0"
author: Gianluca Arbezzano
author_url: https://twitter.com/gianarb
date:   2015-11-28 22:24:50
categories: core release
---
Penny PHP Framework 0.7.0 is ready!

* [[#104]](https://github.com/pennyphp/penny/pull/104) set off email notification on .travis.yml
* [[#106]](https://github.com/pennyphp/penny/pull/106) remove __construct() from PennyEventInterface
* [[#107]](https://github.com/pennyphp/penny/pull/107) Update getting-started.md
* [[#108]](https://github.com/pennyphp/penny/pull/108) Use skeleton app and not classic app
* [[#110]](https://github.com/pennyphp/penny/pull/110) use "phpunit/phpunit": "^4.8|^5.0" in composer.json
* [[#111]](https://github.com/pennyphp/penny/pull/111) update package dependencies
* [[#114]](https://github.com/pennyphp/penny/pull/114) update docs regarding container and path role config
* [[#115]](https://github.com/pennyphp/penny/pull/115) remove dependency status badge
* [[#116]](https://github.com/pennyphp/penny/pull/116) Fixes penny-skeleton-app link
* [[#112]](https://github.com/pennyphp/penny/pull/112) Event Manager split interface
* [[#117]](https://github.com/pennyphp/penny/pull/117) Add EventManager docs
* [[#120]](https://github.com/pennyphp/penny/pull/120) added cakephp eventmanager proxy ( uses trigger->(PennyEventInterface $event) )
* [[#122]](https://github.com/pennyphp/penny/pull/122) Added missing $container property in Dispatcher class
* [[#123]](https://github.com/pennyphp/penny/pull/123) add missing properties in CakeEvent
* [[#124]](https://github.com/pennyphp/penny/pull/124) Fixes deprecated attach() method on Cake EventManager, use on() instead
* [[#125]](https://github.com/pennyphp/penny/pull/125) make scrutinizer score 10
* [[#128]](https://github.com/pennyphp/penny/pull/128) documentation improvements
* [[#127]](https://github.com/pennyphp/penny/pull/127) add php 7 to allow_failures in travis
* [[#126]](https://github.com/pennyphp/penny/pull/126) Fixes wrong namespace in PennyTest\Event
* [[#131]](https://github.com/pennyphp/penny/pull/131) Added missing docblock
* [[#130]](https://github.com/pennyphp/penny/pull/130) rename event adapters
* [[#129]](https://github.com/pennyphp/penny/pull/129) Move repetitive trigger with event to separate private method
* [[#132]](https://github.com/pennyphp/penny/pull/132) Fixes scrutinizer issues
* [[#133]](https://github.com/pennyphp/penny/pull/133) Fixes App::getEventManager() docblock
* [[#134]](https://github.com/pennyphp/penny/pull/134) usage of PennyEvmInterface for docblock instead
* [[#135]](https://github.com/pennyphp/penny/pull/135) refactor Dispatcher
* [[#136]](https://github.com/pennyphp/penny/pull/136) listener call priority in PennyEvmInterface
* [[#137]](https://github.com/pennyphp/penny/pull/137) more improvements
* [[#138]](https://github.com/pennyphp/penny/pull/138) Increase Scrutinizer anaytics
* [[#141]](https://github.com/pennyphp/penny/pull/141) Fixes RouteInfoInterface type hint in handleRoute() method
* [[#142]](https://github.com/pennyphp/penny/pull/142) Fix 139
* [[#143]](https://github.com/pennyphp/penny/pull/143) re-create 141

[Github Millestone](https://github.com/pennyphp/penny/releases/tag/0.7.0)
