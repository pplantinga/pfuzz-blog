---
layout: post
title: Classes and Templates
date: 20 Jan 2014 14:47:00
tags:
- delight
- release
- object orientation
---

I just tagged my first release in Delight! And in Github for that matter.

Version 0.1-alpha is still pre-release, but it's a step in the right direction. It includes support for classes and templates.

{% highlight D %}
class Woodchuck:
	int teeth = 2

	method bite( int tree ):
		return tree - teeth

class Beaver(T):
	T teeth

	method bite( T tree ):
		return tree - teeth

procedure main:
	Woodchuck w = new Woodchuck()
	Beaver!int b = new Beaver!int()
{% endhighlight %}

Check it out at [github.com/pplantinga/delight](http://github.com/pplantinga/delight) and report any bugs!

**Edit:** I've also added some support for enums and structs and inheritance:

{% highlight D %}
enum Cards { Clubs, Diamonds, Hearts, Spades }

struct building:
	int windows
	int doors
	int floors

class BabyWoodchuck <- Woodchuck:
	this():
		super()
	method bite( int tree ):
		return tree - teeth / 2
{% endhighlight D %}
