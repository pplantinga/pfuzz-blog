---
layout: tag-archive
title: "Delight Programming Language"
archive-tag: 'delight'
---

This language aims to provide many of the awesome features of the [D programming language](/archives/d-programming-language.html) but with syntax akin to that of [python](/archives/python.html). Here's a sample:

{% highlight python %}

function add( T a, b -> T ):
	return a + b

procedure main:

	# Dictionary
	auto a = ["a": 1, "b": 2, "c": 3]

	auto x

	# Pythonic for loop
	for key, item in a:

		# Switch requires no "break"
		switch key:
			case "a":
				x += add( item, 4 )

			# b and d lumped together
			case "b":
			case "d":
				x += item - 1
			default:
				x = 5 + item
	
	# Conditional
	if x less than 20 and x in 5 .. 22:
		x *= 2

	# print statement
	print x
{% endhighlight %}

Read [dlang.org](http://dlang.org) for the advantages of using D, many of which apply to delight, since delight uses dmd to compile the code. Delight is just an alternative syntax.
