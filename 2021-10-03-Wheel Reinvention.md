# Wheel Reinvention

The wheels that need the most reinventing are our habits based on old biases, e.g. languages and operating systems.  The old biases - CPUs are expensive, memory is scarce and expensive - are no longer true. 

In this week-long jam (the Wheel Reinvention Jam), I accomplished a lot of what I set out to do (I certainly have not finished and will continue):
- to think about and list the lessons we've learned from building GPLs and OSs (General Purpose Programming Languages, and, Operating Systems,resp.)
- to work on concrete tools that were suggested by the lists.

I argue that we should deprecate the notion of GPLs and OSs and free our minds to think of bigger and better ways to control computers.

# Wrapup
- <u>General</u>
    Overview
	List Programming The Good Parts
    List Programming The Bad Parts
	Other Technologies
	New Perspectives
	
- <u>Concrete</u>
    *Code*
         PFR
    	 code related to "CALL RETURN Spaghetti", in JS, in CL, in Python
    ​     PE - Architecture Diagram

    *Essays*
        Free Your Mind
        We Don't Need Programming Languages Nor Operating Systems
        Control Flow is Orthogonal to Data Structuring
        LEGO Software
		Concurrency
        DaS II
        Typed Packet

- Github

    https://github.com/guitarvydas/wheelreinvention

# Concrete Tools + Drawings

#### PFR

`pfr grammar-file replacement-script <input-file`

- "Parsing" GREP + "parsing sed" (Parsing Find and Replace)
- Based on Ohm-JS
- currently blocked on syntactic silliness, e.g. `await` (due to my unfamiliarity with JS) (I welcome help)
- [WIP](https://github.com/guitarvydas/firstclasscomments).  (Firstclasscomments is an extension of my langjam entry, which shows how to compile diagrams to code).

DLLs can be subsumed by HTTP servers.

Libraries can be subsumed by HTTP servers.

GREP and SED and AWK can be subsumed by something that does better-pattern-matching than simple REGEXPs.  

OTOH, REGEXPs can be specified in one line of code, and, anything "better" requires more lines of code.  

Ohm-JS (based on PEG) seems like a viable choice for this kind of thing.

Currently, DLLs and libraries are "more efficient" than (localhost) HTTP servers.  In fact, the concepts of DLL and library are "optimizations" of the more general concept of "server".  If we replace DLLs and libraries with localhost servers, someone will come up with a way to optimize and speed up localhost servers. 

"Build it and they will come".  

DLLs and libraries are merely premature optimizations of a more general concept.

#### CALL RETURN Spaghetti Code

[CALL RETURN Spaghetti](https://guitarvydas.github.io/2020/12/09/CALL-RETURN-Spaghetti.html)

[code (sync versions in JS, Python, CL, async versions in JS and CL)](https://github.com/guitarvydas/callreturnspaghetti)

### Architecture Diagram of PE

[Architecture Ideas for PE](https://github.com/guitarvydas/wheelreinvention/blob/master/PE-Programming-Enironment-Sketch-Page-1.png)

[Current Technologies that can be applied to PE](https://github.com/guitarvydas/wheelreinvention/blob/master/PE-technologies.png)

PE means Programming Environment (a generalization of IDE).

Basically, I argue that everything that is currently "done at compile time" should be done in the PE. 

That includes macros, includes, OO inheritance, type checking, syntax checking, like-except, DRY, etc., etc.

Everything else can be done at runtime. 

For example, code, dynamic type checking, dynamic object construction (aka Prototype inheritance) can be done at runtime.

Languages are subsumed by the PE.

Code is contained in LEGO®-like Components.

Operating Systems are subsumed by the PE.

Operating Systems are subsumed by CAD-like tools in the PE for plumbing Components together.  For example, if an app needs input from the keyboard, we plug a *keyboard* Component into the app (via the PE).  If the app needs input from a mouse, we plug a *mouse* Component into the app (via the PE).  If an app needs to handle files, we plug a *file system* Component into the app. And so on.

### Essays
[Free Your Mind](https://guitarvydas.github.io/2021/10/02/Free-Your-Mind.html)

[We Don't Need Programming Languages Nor Operating Systems](https://guitarvydas.github.io/2021/09/29/Programming-Languages-and-OSs-Not-Needed.html)

[Control Flow is Orthogonal to Data Structuring](https://guitarvydas.github.io/2021/10/01/Control-Flow-is-Orthogonal-to-Data-Structuring.html)

[LEGO Software](https://guitarvydas.github.io/2021/10/02/LEGO-Software.html)

[Concurrency](https://guitarvydas.github.io/2021/10/01/Concurrency.html)

[Two Syntaxes For Every Language II](https://guitarvydas.github.io/2021/10/02/Two-Syntaxes-For-Every-Language-II.html)

[DaS II](https://guitarvydas.github.io/2021/10/02/DaS-II.html)

[Typed Packet](https://guitarvydas.github.io/2021/10/03/Typed-Packet.html)

## General

I wrote my "thinking" and notes in Scrivener.

Below, I include screenshots of the outlines...

The originals can be found in github [wheel reinvention](https://github.com/guitarvydas/wheelreinvention).

#### Overview

<img src="https://github.com/guitarvydas/wheelreinvention/blob/master/Overview%20-%20Screen%20Shot%202021-10-01%20at%2012.09.26%20AM.png?raw=true" alt="Overview - Screen Shot 2021-10-01 at 12.09.26 AM.png" style="zoom:67%;" />

#### Programming - The Good Parts

<img src="https://github.com/guitarvydas/wheelreinvention/blob/master/Programming%20-%20The%20Good%20Parts%20-%20Screen%20Shot%202021-10-01%20at%2012.09.41%20AM.png?raw=true" alt="Programming - The Good Parts - Screen Shot 2021-10-01 at 12.09.41 AM.png" style="zoom:67%;" />

#### Programming - The Bad Parts

<img src="https://github.com/guitarvydas/wheelreinvention/blob/master/Programming%20-%20The%20Bad%20Parts%20-%20Screen%20Shot%202021-10-01%20at%2012.09.55%20AM.png?raw=true" alt="Programming - The Bad Parts - Screen Shot 2021-10-01 at 12.09.55 AM.png" style="zoom:67%;" />

#### Other Technologies

<img src="https://github.com/guitarvydas/wheelreinvention/blob/master/Other%20Technologies%20-%20Screen%20Shot%202021-10-01%20at%2012.10.09%20AM.png?raw=true" alt="Other Technologies - Screen Shot 2021-10-01 at 12.10.09 AM.png" style="zoom:67%;" />

#### New Perspectives

<img src="https://github.com/guitarvydas/wheelreinvention/blob/master/New%20Perspectives%20-%20Screen%20Shot%202021-10-01%20at%2012.10.49%20AM.png?raw=true" alt="New Perspectives - Screen Shot 2021-10-01 at 12.10.49 AM.png" style="zoom:67%;" />



# What Matters?

There is only one thing that matters:
	1.	controlling machines[^1]

We resort to things that we call:
- paradigms
- experience.

Programming languages are merely syntactic sugar for the above.

Can we create a toolbox of paradigms, then drape syntactic sugar over the paradigms?

Yes.

[^1]: Machines that we call "computers".

# Programming Languages

The concept of programming languages, especially GPLs (General Purpose Languages), should be deprecated.

GPLs are obviated by Ohm-JS(PEG)-based notations.

# Operating Systems

OSs are merely glorified libraries (which can be obviated by using better library technology (e.g. LEGO®-like blocks). 

# Other Biases

There are many other biases, such as 

- the idea that GPLs (General Purpose Programming Languages) must be based on grids of non-overlapping bitmaps (aka Characters, Text).
- 2D notation.
    Until now, we had only paper (pencil-and-paper) to use when evolving ideas.
    Now, we have 3D workstations.

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
