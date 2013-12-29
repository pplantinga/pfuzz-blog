---
layout: post
title: "Static Webpage Analogies"
date: 28 Dec 2013 11:34:00
tags:
- jekyll
- static webpages
- compiled vs interpreted
- the data-code spectrum
---

I've been experimenting with Jekyll in order to get this blog up and running, so here is a blog post on my thoughts about the process.

About Jekyll
------------

In case you don't know, Jekyll is a clever system for managing content that doesn't rely on a database, like most CMS's do, but instead generates and serves static pages. It has a templating system, so it is easy to change all the layouts at once, choose different layouts for different types of content, and all the other things that you'd expect a CMS to do. But it stores the end result instead of the components.

I've already collected a few of my thoughts about static webpages here at the [static webpage tag archive page](/archive/static-webpages.html), but I've also come up with a few analogies that I want to try out.

Static Webpages as Compiled Code
--------------------------------

The first analogy is that static websites are like compiled code, whereas dynamic websites are more like interpreted code. Think about it:

* Speed: compiled code is usually faster, just like static pages.
* Timing: jekyll creates webpages which users later use, like compiling, whereas drupal creates pages on-the-fly, like interpreting.
* Flexibility: dynamic websites, like interpreted code, have more tools available than static websites and compiled code do.

So it's ironic that Jekyll is written in ruby, an interpreted language, and MySQL is written in C, a compiled language (though I've conveniently forgotten to mention PHP). You can also read more about [compiled vs. interpreted languages](/archives/compiled-vs-interpreted.html).

Static Webpages as Data
-----------------------

If you don't know already, [data and code are not two separate things](/archives/data-code-spectrum.html), as much as we try to pretend otherwise. Web developers talk a lot about we need to keep "presentation" and "content" separate, which to me sounds like "code" and "data."

So while we can't say that static webpages are data while dynamic webpages are code, it is still helpful to say that static webpages are more like data and dynamic webpages are more like code. And markdown files are more like data and the templates are more like code. Jekyll does a great job of separating content from presentation.  

I have to say that the data-centered approach has helped me focus more on the content, which is where the focus should be. For example, I'm making the tag archive pages individually, which means I can include valuable information on them, unlike if they were automatically generated (don't worry, I don't have to update them all each time I write a new post).

Let me know in the comments what you think of these analogies and if you can think of other ones!
