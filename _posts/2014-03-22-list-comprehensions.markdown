---
layout: post
title: List Comprehensions!
date: 22 Mar 2014 11:51:00
tags:
- delight
- python
- list comprehensions
---

One feature of Python and Haskell (which make up 2/3 of my favorite languages) that is not in D (the last of my fav's) is list comprehensions. These are fricken sweet, so I decided that it needed to go into Delight. So here it is!

You can now include a list comprehension as follows:

{% highlight python %}
procedure main:
	auto list_comp = { x * 2 for x in 0 .. 10 by 2 where x ^ 2 more than 3 }

	print list_comp
{% endhighlight %}

This'll spit out:

	[ 4, 8, 12, 16 ]

Pretty sweet, eh?
