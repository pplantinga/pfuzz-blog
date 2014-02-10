---
layout: post
title: Delight Testing and Errors
date: 10 Feb 2014 21:49:00
tags:
- delight
- debug
---

I've been in 哈尓滨 and 崑山 for the past few weeks, so I've not had time to work on the language or post here. So here's the latest news since I've been back. Bugfixes and some small features: unittests and error handling.

{% highlight D %}
unittest:
	assert 3 less than 4
	assert 5.0 equal to 5.0
	try:
		assert 6 less than 5
	except Exception e:
		assert 5 not more than 5
	finally
		assert 4 less than 5
{% endhighlight %}
