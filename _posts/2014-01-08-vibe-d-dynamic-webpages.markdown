---
layout: post
title: Vibe.d Dynamic Webpages
date: 8 Jan 2014 10:19:00
tags:
- Vibe.d
- static webpages
- compiled vs interpreted
---

In my [discussion on static webpages](/archives/static-webpages.html) I wrote down a bunch of reasons why static webpages are much better in some situations than dynamic webpages. I wrote a lot about how if you just have the right tools (aka jekyll and co.) you can manage many of the shortcomings of static webpages without giving up their benefits. I also wrote a lot about the shortcomings of dynamic webpages.

I guess I've found a tool that manages many of the shortcomings of dynamic webpages, called [vibe.d](http://vibed.org) which is written in D. Go to the website to read the full list of advantages, but here are a few:

* Blazingly fast - The server is compiled (obviously) and is built on [fibers](http://dlang.org/phobos/core_thread.html#.Fiber) (sometimes called co-routines).
* Diet templates - HAML done right, plus using D code inside. One fewer language out of the unholy web development mix to worry about. 
* Database support - Of course, it wouldn't be dynamic webpages otherwise.
* Simple API - Easy things are easy, hard things are possible.

There are more features coming that I'm excited about, but I'll leave it at this for now. Now if only I had my own dedicated server machine...
