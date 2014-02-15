---
layout: post
title: The "in" Operator
date: 15 Feb 2014 13:08:00
tags:
- delight
- python
---

"in" is just one small word, but it can make a big difference. In python it is easy to find stuff in arrays, since the language includes the "in" operator:

{% highlight python %}
if 4 in [0, 2, 4]:
	print "hello"
{% endhighlight %}

Walter Bright (the creator of D) didn't include this operator, since "in" is an O(n) operation. It's fairly easy to replicate with standard library functions, such as canFind. It's frustrating though that there isn't one that works with all foreach-able types (not even all arrays). 

I've decided to include this operator, even though it may slow down performance a bit due to overuse. It's just so handy to have!
