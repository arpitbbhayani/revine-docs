---
title: Teleport
seq: 3.3
---

Every [shape](/docs/shapes) can teleport to any point in the [canvas](/docs/canvas) using the `teleport` command. For example, to teleport a rectangle named `block` to point `(200, 200)`, the command we write is

```
block.teleport(200, 200)
```

![Revine Teleport Example](https://user-images.githubusercontent.com/4745789/153819291-cc1d6f6e-8bfd-4045-9953-324cf9c1de1f.gif)

a general syntax for invoking move is

```
<name of shape>.jump(<distance>)
```

## Example

To make the `block` teleport to `(200, 200)` when the key `w` is pressed we write

```
shape block(rectangle):
  .color = RED
  .position = (100, 100)
  .fill = RED
  .width = 25
  .height = 65
endshape

onkey w
  block.teleport(200, 200)
endonkey
```
