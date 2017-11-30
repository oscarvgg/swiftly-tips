---
title: #1 Closure retain cycle
date: 2017-11-30 20:07:08
tags: memory
---

Avoid calling `self` inside your closure as much as possible.

```swift
let tower = { [weak self] rapunzel in
  return self?.knight.save(rapunzel)
}
```

What if `self` is `nil`? I know what you're thinking. Forget `unowned`! Just pass a capture list with the properties you need inside the closure.

```swift
let tower = { [knight] rapunzel in
  return knight.save(rapunzel)
}
```

And that is how it is done.