---
layout: post
title:  "Free Your Mind"
---

# Elephant in the Room

Computers are asynchronous.

Period.

# Async vs. Sync

Trying to program computers using synchronous methods is a *tactic*.

Over-using the synchronous tactic will cause accidental complexity, for example callback-hell, etc.

# Step 1 Before Step 2

Most people (non-programmers) already understand asynchronous processes.

For example, *cooking recipes* are often arranged in an asynchronous manner:

1. Boil the potatoes. 
2. While the potatoes are boiling, chop up ..."

Five (5) year-old children are taught hard realtime notations

- piano lessons
- music scores.

CEOs understand asynchrony inherently and use *whiteboards* to communicate their intentions.

CEOs don't want to be bothered by the enigneering details.  This *does not* mean that they are ignoring the details, just deferring them (to Architects and Engineers).  Our notations *can* deal with *all* of the details while presenting less detail at each step - using layers.  *Provenance* can be accomplished in layers.

# Control-Flow

Asynchrony is about control-flow.

OO does not express Control-flow conveniently.

FP does not express Control-flow conveniently.

Rendezvous multi-tasking does not express Control-flow conveniently (rendezvous is merely another tactic for reducing async problems into sync problems by essentially ignoring the async portion).

CPS (Continuation Passing Style) does not express Control-flow conveniently.  CPS is, basically, GOTO in disguise.  Yes, GOTO *can* express control-flow, but it isn't convenient.  Yes, CPS *can* express control-flow, but it isn't convenient.

# Multiple Syntaxes

This leads into the notion of decoupling syntaxes - one syntax for data structuring, another syntax for control-flow structuring. [Two Syntaxes For Every Language II](https://guitarvydas.github.io/2021/10/02/Two-Syntaxes-For-Every-Language-II.html) and so on.

Different syntaxes for:

- Implementation, vs.,
- Use[^1]

[^1]: Use is also known as scripting.

# One Language To Rule Them All

One Language to Rule Them All is a bad idea.

This approach closes the mind.

The idea of GPL (General Purpose Language) falls into this category.  Use SCNs[^2] instead of GPLs.

[^2]: SCN is Solution-Centric-Notation.

# How to Express Async?

## Statecharts

[Statecharts Presentation  (Papers We Love)](https://guitarvydas.github.io/2020/12/09/StateCharts.html)

[Harel's Original Paper](https://www.inf.ed.ac.uk/teaching/courses/seoc/2005_2006/resources/statecharts.pdf)

[Statecharts Again](https://guitarvydas.github.io/2021/02/25/statecharts-(again).html)

## Drakon

[Drakon Editor](http://drakon-editor.sourceforge.net)

## FBP

[Flow Based Programming](https://jpaulm.github.io/fbp/)

## ASCs - Asynchronous Software Components

(see my [Blog](https://guitarvydas.github.io/2021/09/21/Table-of-Contents-Sept-17-2021.html), search for "Isolation", Software Components", "Software Components 101", "ASC", "DaS", etc., etc.)

## Diagrams (DaS)

Diagrams of asynchronous components can form control-flow-based paradigms.

Diagrams built using the synchronous paradigm tend to fail.  Such diagrams are harder to build and are often less meaningful.  This (synchrony) has led to the (untrue) notion that node-and-arrow diagrams don't work.

# See Also

[Blog](https://guitarvydas.github.io)
[Table of Contents](https://guitarvydas.github.io/2021/09/21/Table-of-Contents-Sept-17-2021.html)
[Videos](https://www.youtube.com/channel/UC2bdO9l84VWGlRdeNy5)

[SCN](https://guitarvydas.github.io/2021/04/10/SCN.html)

[References](https://guitarvydas.github.io/2021/01/14/References.html)

<script src="https://utteranc.es/client.js" 
        repo="guitarvydas/guitarvydas.github.io" 
        issue-term="pathname" 
        theme="github-light" 
        crossorigin="anonymous" 
        async> 
</script> 
