---
title: Nº 4 - Using variadic parameters
date: 2018-04-24 11:28:13
tags:
  - style
  - syntax
---

Want your array parameters to look way cooler?

## Boring

```swift
func trapInUpsideDown(people: [String]) {
  // ... your code here
}

trapInUpsideDown(people: [“Dustin”,”Mike”,”Lucas”, "Will"])
```

## Cooler look

```swift
func trapInUpsideDown(_ people: String...) {
  // ... your code here
}

trapInUpsideDown(“Dustin”,”Mike”,”Lucas”, "Will")
```
😉
