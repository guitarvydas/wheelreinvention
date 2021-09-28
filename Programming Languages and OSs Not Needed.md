---
layout: post
title:  "We Don't Need Programming Languages Nor Operating Systems"
---

# Programming Languages:
There are only 2 important things for programming computers:

1. Getting computers to do what we want (e.g. using computing machines to augment human capabilities).

2. Paradigms.

Programming Languages fall in between 1 & 2.

One can do away with programming languages and replace them with simpler "notations" using Ohm-JS (PEG).

I think of notations as very simple DSLs.

It should take only 10's of minutes to produce a notation. 

Notations can be tuned to a particular problem (something Physicists do). 

Multiple Notations can be used on a single problem. 

Notations can be transpiled into other languages (I call them Toolbox Languages), like Python, JavaScript, Common Lisp, etc. 

Notations are like "new" compilers - instead of compiling to assembler, notations compile to Toolbox Languages.

# Operating Systems
Operating systems are just libraries.

One feature that OSs provide is multitasking. 

The kind of multitasking they provide is rife with accidental complexity - "we're going to make this square peg fit our notation even if it kills us".

For example, current OSs provide require us to deal with thread safety. 

Thread safety is accidental complexity caused by the use of memory sharing. Memory Sharing is used only due to old-fashioned premature optimization (CPUs and Memory used to be expensive in the 1950's). 

If we build computing devices using many rPIs, each running exactly one program (no Linux), then thread safety becomes a non-issue. 

Poof.

Another feature that OSs provide is honest-to-goodness big lumps of library code, like file handling. 

That stuff can simply be moved into LEGO(R) components that replace the concept of libraries. 

No OS needed for this, either. 

Poof.

# LEGO(R) Block Software

The keys to making LEGO(R) block software are:

- isolation
- concurrency.

Isolation gives you "build and forget".  No dependencies.

Concurrency means that blocks can run in any order (and, therefore, can be snapped together in any order to make different apps).

[It might be helpful to think of building everything using networks of rPIs or to think that EVERY function runs in its own thread. (That's not actually far-fetched if you know about anonymous functions and callbacks).]

# The Universal Acid

Isolation is a Universal Acid[^1]: - it eats through old-fashioned ideas.

Isolation implies concurrency. 

Software Components in an app must be written in such a way that order cannot matter. 

Components from one app can be re-ordered to form a new app.

# Sightings of Isolation

Isolation can be seen in UNIX threads.

Isolation can be seen in Worlds (,,,).

[FYI - Functions do not enforce Isolation, OO does not enforce Isolation, and so on.]

[^1]: Term borrowed from Daniel Dennett.

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
