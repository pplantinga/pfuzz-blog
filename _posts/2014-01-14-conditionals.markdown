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
if x equals y or y equals z:
	x = z
else if x less than y and y greater than z:
	x = y + z
else if x in 0 .. 12:
	x = 13
else:
	x = 1
{% endhighlight %}

Instead of using the confusing == operator, I'll just use the keyword equals. There should also be keywords for < and > for consistency and readability since < and > can be confusing. The only questions I have are: "How useful are '<=' and '>='? Can I leave them out without ruining the language?"

Let me know what you think!
