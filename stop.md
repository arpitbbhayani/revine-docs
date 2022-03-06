---
title: Stop
seq: 1.6
---

To stop the infinite animation [loop](/docs/loop) you can invoke the command `stop()`. As soon as the command is executed the infinite animation loop will stop and the animation will freeze in the moment.

In the example below, we have the text "Hello" that is moving constantly to the right. We have added an [onkey](/docs/onkey) interaction that says, as soon as the key "s" is pressed stop the loop. When you run the code below and press key "s" the loop will stop and the animation/game will freeze.

```
shape greeting(text):
  .text = "Hello"
  .color = RED
  .position = (100, 100)
endshape

onkey s
  stop()
endonkey

loop
  greeting.move(RIGHT)
endloop
```

![Revine Stop Example](https://user-images.githubusercontent.com/4745789/156917711-fba54e6b-0a79-4c7c-be70-ec5fb04c64d0.gif)
