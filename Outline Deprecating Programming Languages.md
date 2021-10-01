Title: Deprecating Programming Languages  
Author:

   The concept of programming languages, especially GPLs (General Purpose Languages), should be deprecated.
   
   There is only one thing that matters:

1. controlling machines[^fn1]

We resort to things that we call:
- paradigms
- experience.

Programming languages are merely syntactic sugar for the above.

Can we create a toolbox of paradigms, then drape syntactic sugar over the paradigms?  

Yes.


       Several ideas hurt computing progress:

* computers are functions (detrimental idea)
* there is one programming language to "rule them all" (detrimental idea)
* concurrency must be avoided (detrimental idea)

    


       I plan to:
       

1. list beneficial concepts that we have discovered through the development of various languages
2. list anti-beneficial concepts that have permeated our programming languages
3. list other technologies
4. suggest new perspectives 
5. suggest little tools based on the above ideas (e.g. replace DLLs with servers, replace GREP with a parsing-grep, replace subroutine libraries with Components, etc.)
6. Build prototypes for the tools suggested in (5) above.

    


    The goal is to produce a PE (programming environment) that

* supports transpiling diagrams to code
* supports transpiling text to code
* support multiple notations, e.g. a grammar specification and a rewrite specification for every notation
* concurrency as the default
* macros (same as "mutiple notations" above)
* include
* like

    


           There is no such thing as essential complexity.
           
           There are only problems-to-be-solved.
           
           Problems can be made to seem more complex by choosing poor notations for describing the problems and their solutions.
           


               For example, most of our programming languages (including /bin/*sh) treat concurrency as something to be avoided.  
               
               Special syntax is required to denote concurrency, e.g. "&" in /bin/*sh.  
               
               Concurrency is implicitly treated as a second-class feature.
               
               Programmers now believe that concurrency is a "hard problem".
               
               We have seen "reasoning" about concurrent systems break down, e.g. the Mars Rover disaster.
               
               Even lowly JavaScript mistreats concurrency.
               
               We believe that network outages are "failures".
               
               Network outages are actually part of the problem-to-be-solved.  Our current crop of GPLs forces us to think of outages as errors instead of part of the problem.
               
               Happy Path culture.

   - isolation obviates most epicycles we have invented
   - isolation solves dependency problems - they can't happen, except via mailboxes, no memory sharing
   
   - FP provides pseudo-isolation by prohibiting mutability
   - UNIX essentially produced concurrent sandboxes for every command, nothing in the command code could affect other commands (assisted by hardware ; distributed computing (e.g. multiple rPis) results in the same kind of sandboxing)

   - parts of programming can be described using mathematical notation
   - but, only parts


   - mathematics can describe some of programming, but not all of programming
   - programming is machine control and sequencing
   - mathematics describes functions - input always leads to output - but programming describes something more (input and no output - see Asynch Thinking)

   - left to others

   - merely libraries that help with avoidance of concurrency

[^fn1]: Machines that we call "computers".