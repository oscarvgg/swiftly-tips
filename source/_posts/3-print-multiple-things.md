---
title: Nº 3 - Printing multiple variables at once?
date: 2018-04-24 11:15:33
tags: style
---

Wanna print multiple variables?

## Problem

```swift
let name = "Tony"
let lastName: "Stark"

print(name)
print(lastName)
```

## Better solution

Wrap them on a tuple.

```swift
let name = "Tony"
let lastName: "Stark"

print((name, lastName))
```

Awh, syntactic sugar ☺️