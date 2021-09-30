---
layout: post
title:  "We Don't Need Programming Languages Nor Operating Systems"
---

# Reinventing the Wheel

There are only 2 things that are important for programming computers:

1. Getting computers to do what we want (using computing machines to augment human capabilities).

2. Paradigms.

# Programming Languages:

Programming Languages fall in between 1 & 2.

One can do away with programming languages and replace them with simpler "notations" using Ohm-JS (PEG).

I think of notations as very simple DSLs.

It should take only 10's of minutes to produce a notation. 

Notations can be tuned to a particular problem (this is something that Physicists do). 

Multiple Notations can be used on a single problem. 

Notations can be transpiled into other languages (I call them Toolbox Languages), like Python, JavaScript, Common Lisp, etc. 

Notations are like "new" compilers - instead of compiling to assembler, notations compile to Toolbox Languages.

# Operating Systems
Operating systems are merely libraries.

One feature that OSs provide is multitasking. 

The kind of multitasking they provide is rife with accidental complexity - "we're going to make this square peg fit our notation even if it kills us".

For example, current OSs incur issues with thread safety. 

Thread safety is accidental complexity caused by the use of memory sharing. Memory Sharing is used only due to old-fashioned premature optimization (CPUs and Memory used to be expensive in the 1950's). 

If we build computing devices using many rPIs, each running exactly one program (no Linux), then thread safety becomes a non-issue. 

Poof.

Another feature that OSs provide is honest-to-goodness big lumps of library code, like file handling. 

That stuff can simply be moved into LEGO(R) components that replace the concept of libraries. 

No OS needed for this, either. 

Poof.

OSs provide the concept of DLLs (shared libraries).  We use those every day in another form - HTTP servers (servlets).

Servlets currently aren't as "efficient" as DLLs, but they would be if we insisted on using them instead of DLLs.  

[The "build it and they will come" syndrome has happened many times in computering - from Assembler to HLLs (gcc), C++ used to be too inefficient to use on ubiquitous computing platforms of the day (e.g. 8-bit micros), etc, etc].

[Note that DLLs are not "free".  The OS must load them and fix up all of the holes. Then, the DLLs need to be mapped into the address space of the application(s) using them.] 

Poof.

# Paradigms

Concepts such as OO and FP and Structured Programming, etc. are based on research and experience.

They are often presented using their own syntax that *look* like languages.

Let's take OO for example. OO was popularized by Smalltalk but quickly branched into various syntaxes, e.g. C++, Eiffel, CLOS, JS, Python, etc.

The underlying principles are mostly the same, but the syntax is different in each variant.

Another example: FP first appeared in 1956 in the form of Lisp.  Today, FP looks nothing like Lisp, but, the underlying principle (the Paradigm) is the same.  (I might argue that today's syntax first appeared APL, but that's an aside).  The major delta between 1956 and now is "just" syntax (there have been improvements - more experience - with the paradigm, but the new syntax obscures the improvements).

I argue that it is easy to create syntax and just as easy to throw it away as new experience is gained with the paradigm.

I argue that this same strategy - inventing syntax - should be applied to problems-to-be-solved and not just to paradigms.

[It is a good idea to keep a checklist handy of what we've learned to be good and what we've learned to be bad, as one invents new syntax].

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

Isolation can be seen in Worlds (http://vpri.org/pdf/rn2008001_worlds.pdf).

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
