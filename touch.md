---
title: Touch
seq: 4.2
---

Revine provides a way to detect and handle when the two [objects](/docs/objects) touch each other or not. You can use `touch` on the two objects as shown below

```
box1.touch(box2)
```

The `touch` function returns a boolean value `True` if the objects touch other and `False` otherwise. You can use the [touch](/docs/touch) statement with the soon-to-be-launched [if](/docs/if) statement to check for collision and then take some actions as per the state.
