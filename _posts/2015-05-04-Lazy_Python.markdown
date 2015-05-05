---
layout:     post
title:      "How to be lazy with Python"
subtitle:   "The usage of lambda and recursion in python"
date:       2015-05-05 12:00:00
author:     "Binghuan Lin"
header-img: "img/post-bg-02.jpg"
---
<u>First, this post is not aim to achieve the best algorithm, in terms of complexity, for the examples provided below.</u>

It might happen in a technical interview, you were asked to write a python program for .. in one line?

This is about how to create anonymous functions in Python. To do that, you can use `lambda` function.

Here are two simple examples of how to use `lambda` and recursion to achieve that.

## Example 1: Fibonacci Sequence

    fibo = lambda N, x=0,y=1: x if not(N) else fibo(N-1,y,x+y)


## Example 2: Square Root

    mySQRT = lambda x, ans=1., epsilon=0.01: ans if abs(ans**2-y)<epsilon else mySQRT(x,1./2*(ans+x/ans),epsilon)


<p>Photographs by <a href="https://www.flickr.com/photos/nasacommons/">NASA on The Commons</a>.</p>