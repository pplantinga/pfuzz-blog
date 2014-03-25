---
layout: post
title: Scope Guard
date: 25 Mar 2014 09:30:00
tags:
- delight
- d programming language
- scope guard
---

Cool new feature: [scope guards](http://dlang.org/statement.html#ScopeGuardStatement). These ensure that your code will be run upon exit from scope.

{% highlight D %}
function add(T a, b):
	scope exit:
		assert a less than b
	return a + b
{% endhighlight %}

There's also `scope success` and `scope failure` like in D. I've decided that this feature obviates the need for [contract programming](/2014/03/13/0.1-beta2.html), so I've removed that feature.
