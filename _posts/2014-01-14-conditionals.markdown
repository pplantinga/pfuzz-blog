---
layout: post
title: Conditionals
date: 14 Jan 2014 22:22:22
tags:
- delight
- conditionals
---

Parsing comments turned out to be a lot harder than I thought it would be. But it's done now. The next task is conditionals, which will look quite similar to pythonic conditionals, except for one slight change.

{% highlight python %}
if x equal to y or y not equal to z:
	x = z
else if x not less than y and y more than z:
	x = y + z
else if x in 0 .. 12 or x in [ 0, 2, 5 ]:
	x = 13
else:
	x = 1
{% endhighlight %}

Instead of using the confusing '==' operator, I'll just use the keywords 'equal to'. I still sometimes write '=' instead of '==' which is a hard bug to track down. Also, '<' and '>' become 'less than' and 'more than' for consistency and readability since '<' and '>' can be confusing (at least for me). '>=' and '<=' become 'not less than' and 'not more than' respectively, which are arguably clearer.

Let me know what you think!
