---
title: Loop
seq: 1.5
---

Any movements, actions, animation that needs to be run infinitely should be wrapped in the _loop_ and _endloop_ statements. The statements written within the `loop` will be run one after the other forever. `loop` is the ideal place to write business logic for a game.

For example, to continuously move the word "Hello" to the right you can put the [move](/docs/move) statement in the `loop` as shown below

```
shape greeting(text):
  .text = "Hello"
  .color = RED
  .position = (100, 100)
endshape

loop
  greeting.move(RIGHT)
endloop
```

![Revine Command Example](https://user-images.githubusercontent.com/4745789/136987897-3c66b590-7604-49d0-86bc-7e22dd63e333.gif)
