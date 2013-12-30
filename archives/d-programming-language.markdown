---
layout: tag-archive
title: "D Programming Language"
archive-tag: 'static webpages'
---

I've gotta have a page about my favorite programming language. Seriously this one is awesome. Here is a sample code block, taken from [dlang.org](http://dlang.org).

{% highlight d %}
void main() {
    // Define an array of numbers, double[]. Compiler recognizes the common
    // type of all initializers.
    auto arr = [ 1, 2, 3.14, 5.1, 6 ];
    // Dictionary that maps string to int, type is spelled int[string]
    auto dictionary = [ "one" : 1, "two" : 2, "three" : 3 ];
    // Calls the min function defined below
    auto x = min(arr[0], dictionary["two"]);
}
// Type deduction works for function results. This is important for generic
// functions, such as min below, which works correctly for all comparable
// types.
auto min(T1, T2)(T1 lhs, T2 rhs) {
    return rhs < lhs ? rhs : lhs;
}
{% endhighlight %}

Why do I like this language so much? I think it demonstrates very well that you don't have to give up all the nice features of dynamic lanugages in static languages. Foreach loops and dictionaries happen to be two of my fav's but there are plenty here! D has many of the advantages of both [compiled and interpreted languages](/archives/compiled-vs-interpreted.html).
