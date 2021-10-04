---
layout: post
title:  "Typed Packet"
---

# Overview

A very, very simple example of a typed packet.

# Input
input: 4 bytes
# Output
output: int64

# Initial Verification:
```
if there are 4 bytes remaining in the stream
then
  grab the next 4 bytes
else
  declare error
end if
wrap header and trailer onto the 4 bytes
```

# Tags

tag = flexible number of bytes, last byte has low bit set

for example

`int8 =  00000001`
`int16 = 00000011`
`int32 = 00000101`
`int64 = 00000111`

See early dynamically typed languages for ideas on how best to arrange tags.

See, also, Huffman encoding.

See, also, network packet layout.

# Physical Layer

The *physical layer* carries *bytes* from one Component to another.

Each packet has a header and a trailer, in the form of flexi-tags.

- header (array of bytes terminated by low bit set)
- payload - array of bytes
- trailer - must match the head (exactly)

# ECC

ECC means Error Correcting Code.

We can check the packets using a variety of techniques, at a layer *above* the physical layer.

# Producing Output

In this example, we produce 6 bytes (header, 4 bytes, trailer)

`0x07, ??, ??, ??, ??, 0x07`

output of this stage = 6 bytes

# Network Packets

Note the similarities between this scheme and network packets.

# OSI Model

A useful starting point might be the OSI Model for data packets.

# Validator Components

Some Components "do something" and others simply perform type-checking.

Today, we chop type-checking up into two pieces:

1. input validtation
2. type checking.

# Efficiency

This scheme appears to be inefficient, except when compared to passing JSON character data around in a network.

# Optimization

Is it possible to optimize this model?

We simply perform type-checks in the PE[^1] (at "compile time") as we hook Components up.

This kind of optimization is nothing new.  

We simply move "compile time" into the PE.

[^1]: Programming Environment.

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
