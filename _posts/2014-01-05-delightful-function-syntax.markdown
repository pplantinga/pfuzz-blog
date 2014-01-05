---
layout: post
title: Delightful Function Syntax
date: 5 Jan 2014 16:28:00
tags:
- delight
- whitespace
---

I've been heavily debating the syntax of the language. Here are some ideas I've had...

First, functions are important, how should they look?

To be honest, I like how Ada does it.

{% highlight ada %}
function Count_Letters(Item1, Item2: String) return Natural is
	Count : Natural := 0;
begin
	...
	return Count;
end Count_Letters;
{% endhighlight %}

Of course in our case, indentation declares the scope. What about this?

{% highlight D %}
count_letters takes string item1, item2 returns int:
	int count = 0
	...
	return count
{% endhighlight %}

or a more Haskellian approach:

{% highlight D %}
count_letters: string item1, item2 -> int
	int count = 0
	...
	return count
{% endhighlight %}

And I like calling functions in Haskell. Just use a space! Also, functions have precedence, so you can do things like:

{% highlight haskell %}
max 5 2 * 4 -- returns 20
{% endhighlight %}

Let me know what you think!
