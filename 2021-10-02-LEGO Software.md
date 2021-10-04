---
layout: post
title:  "LEGO® Software"
---

# LEGO®:

Why does LEGO® work?  

Because of its API.

What is LEGO®'s API?

1) exactly one type
2) very simplistic.

LEGO®'s' API is: a round peg.

The lesson for us is: chop types up into layers.  

Have one extremely simple type at the bottom (I favour the tagged event {tag, data}).  

Build the rest of the types up from the bottom (if you squint, you will see that UNIX /bin/*sh already does this - the API is "lines of text".  Other tools, e.g. awk, build up more interesting types (e.g. fields) from that basic transport-layer type.  

 Ohm-JS should make it easy to build languages of types. Hmm, somewhere I think I've written about this, probably https://guitarvydas.github.io/2020/12/09/Type-Stacks.html. 

# Physical Layer Type

There must be ONE type for interchange.  

Hmm, maybe "array of bytes" is that type (basically a non-type until you put more type-filters in the pipeline).

# Type Checkers Are Interpreters

Note that a type-checker is an interpreter.

That interpreter is, currently, a big lump of code that we put into pipeline that we call *compiletime --> runtime*.

# Layered Type Checkers

If you chop up the type-checking interpreter into smaller pieces and pipe them all together, you would get the same effect.

For example, the first piece of type-checking might be to recognize basic types like int8, int16, char, string, lambda, etc, etc.  The second piece might be an arg counter for lambdas (pass all non-lambdas through, unchecked)[^1]

[^1]:[I've been forcing myself to learn Javascript and, I feel that the worst missing feature is arg counting)]  

# Type Checking is Like Syntax Checking

Type checking is an error check like, "end if" syntax, but we're not at the point yet where it is so simple that we tend to forget about it (like "end if" syntax).

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
