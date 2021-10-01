---
layout: post
title:  "Concurrency"
---

# Model of Concurrency

A simple concurrent system is:
- two computers in separate rooms 
- they are connected by a wire
- they send messages to one another
- the messages are one-way only, no "return" is expected.

## Diagram

<img src="/Users/tarvydas/quicklisp/local-projects/wheelreinvention/Concurrency.png" alt="Concurrency" style="zoom:67%;" />

## Everything Else is an Optimization

Every other feature of concurrency is an optimization of this model.

Memory Sharing

Multiple Cores

# Premature Optimization

If you forget (ignore) what the basic model is, you will eventually run into trouble (aka *accidental complexity*).

# See Also

[Blog](https://guitarvydas.github.io)
[Table of Contents](https://guitarvydas.github.io/2021/09/21/Table-of-Contents-Sept-17-2021.html)
[Videos](https://www.youtube.com/channel/UC2bdO9l84VWGlRdeNy5)
[References](https://guitarvydas.github.io/2021/01/14/References.html)

<script src="https://utteranc.es/client.js" 
        repo="guitarvydas/guitarvydas.github.io" 
        issue-term="pathname" 
        theme="github-light" 
        crossorigin="anonymous" 
        async> 
</script> 
