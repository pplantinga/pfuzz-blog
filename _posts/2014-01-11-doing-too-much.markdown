---
layout: post
title: Doing Too Much
date: 11 Jan 2014 11:45:00
tags:
- delight
- russian students
---

I've been working on Delight, but no new language features have happened for awhile. I was going to add the function declaration syntax, but I realized in the middle of it that the changes I were making weren't all related to the syntax. I couldn't keep all the projects straight in my head, so I had to undo all my changes, and go on a refactor binge. This had the added benefit of keeping all the changes separate in the git commit log.

What's ironic is that in real life too I've been doing too much. I offered to teach English to a bunch of Russian students even though I still had grading to do.

I'm finally to the end of both the teaching and the refactoring, so now it's back to work on function declaration syntax. Here's what it's going to look like for now:

{% highlight D %}
function add(int a, b -> int):
	return a + b

procedure main:
	int c = add(a, b)
{% endhighlight %}

Since D has type inference, you'll be able to leave off the return type. And if you replace the "int" with "T" it will automatically become a template.

The "function" means "pure function" or maybe even "const pure function" in D-speak, which basically means no side effects. And "procedure" means "doesn't return anything" though the behavior is easily replicated with a ref parameter. The difference between functions and procedures (and methods once I tackle classes) will hopefully force programmers to be clearer in their heads what they're trying to do, and result in performance gains.
