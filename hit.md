---
title: Hit
seq: 4.2
---

Revine provides a way to detect and handle when the two [objects](/docs/objects) hit each other or not. You can use `hit` on the two objects as shown below

```
box1.hit(box2)
```

The `hit` function returns a boolean value `True` if the objects hit other and `False` otherwise. You can use the [hit](/docs/hit) interaction with the soon-to-be-launched [if](/docs/if) statement to check for collision and then take some actions as per the state.
