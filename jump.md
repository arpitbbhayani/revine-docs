---
title: Jump
seq: 3.2
---

Every [shape](/docs/shapes) can jump in the upward direction by invoking the `jump` command with distance to jump. For example, to jump a rectangle named `block` by `100` units of distance, the command we write is

```
block.jump(100)
```

![Revine Jump Example](https://user-images.githubusercontent.com/4745789/153479168-06795bff-f08d-4be3-b430-95aaddffcc71.gif)

a general syntax for invoking move is

```
<name of shape>.jump(<distance>)
```

## Example

To make the `block` jump when the key `w` is pressed we write

```
shape land(line):
  .color = BLACK
  .point1 = (500, 350)
  .point2 = (0, 350)
endshape

shape block(rectangle):
  .color = RED
  .position = (50, 284)
  .fill = RED
  .width = 25
  .height = 65
endshape

onkey w
  block.jump(40)
endonkey
```
