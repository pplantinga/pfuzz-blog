---
layout: tag-archive
title: "Delight Programming Language"
archive-tag: 'delight'
---

This document, besides recording all posts about Delight, also aims to give a fuller description of the language than the one at [the github page](http://github.org/pplantinga/delight).

Delight aims to provide the best features of the [D programming language](/archives/d-programming-language.html) but with syntax akin to that of [Python](/archives/python.html). Here's a sample:

{% highlight python %}

	#. Block comment scope is determined
		by indentation

	function add( T a, b -> T ):
		return a + b
	unittest:
		assert add( 1, 2 ) equal to 3
		assert add( 1.0, 2.0 ) equal to 3.0

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
		if x less than 20 and x in [ 2, 4, 6, 8 ]:
			x *= 2

		# use () to wrap multi-line expressions
			making sure to end at the same indentation level as you started
		else if (
			x in [ 2, 3, 5 ]
			and x not in [ 4, 6, 7 ]
		):
			x -= 2

		# print statement
		print x
{% endhighlight %}

Read [dlang.org](http://dlang.org) for the advantages of using D, many of which apply to Delight, since Delight is just an alternative syntax. If there's some feature of D that you feel should be in Delight, but isn't, let me know and we'll see if we can add it!

The features are mostly recorded in the blog posts listed below:
