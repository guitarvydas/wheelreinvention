---
layout: post
title:  "Control Flow is Orthogonal to Data Structuring"
---

# Function Call
Is *one* of the choices in describing Control Flow.

# Asynchronous vs. Synchronous
One of the choices in describing Control Flow.

# If Then Else
One of the choices in describing Control Flow.

# Tree, DAG
One of the choices in describing Data Structuring.

# Object / Datum
- scalar data
- lambda

## Promise
- a Promise is a thread 
- a Closure is a snapshot of the data in a thread
- a Continuation is a snapshot of a thread - containing data and code (control flow)
- an Operating System Thread is merely a Continuation (see Greenspun's 10th Rule)

# Control Flow

- pointer to instruction to be executed 
- Program Counter (PC)
- implemented in hardware as an interpreter, made available to software

# Data Structure

- pointers to heap
- pointer to stack (SP)

# Registers

- registers are *shared*, *global* variables implemented in hardware, made available to software
- the PC register is a global variable (shared by all threads on that CPU)
- the SP register is a global variable (shared by all threads on that CPU)
- the MMU is a global variable (shared by all threads on that CPU)

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
