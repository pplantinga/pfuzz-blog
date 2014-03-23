---
layout: post
title: Passthrough
date: 28 Feb 2014 20:20:20
tags:
- delight
- d programming language
---

Today is cool because today's date is cool (2 x 14 = 28). Today is also cool because I just added a new statement to Delight, called "passthrough." I'm doing my best to add the best features of D and leave out the rest. So if there's a feature of D that you want to use, but it's not in Delight, this is the statement for you.

Everything in the scope of this statement will be put into the D code as-is. So now anything that D can do, Delight can do as well :)

Here's an example:

{% highlight D %}
procedure main:
	int i = 5
	passthrough:
		i++;
		for (; i < 20 && i != 4; i++ )
		{
			writeln( "weird" );
		}

	print "cool beans"
{% endhighlight %}
