---
title: Lambda
draft: false
tags:
 - ScriptType
---
# Lambda : [[FunctionBase]]

A Lambda is a small, unnamed function written directly where it's needed, usually handed to another function. List operations such as [[List#^where2061106082\|Where()]] and [[List#^orderby-730234582\|OrderBy()]] take a lambda and run it once for each item — for example `q => q % 2 == 0`. The part before the `=>` names the input, and the part after works out the result.

