---
title: Move
seq: 3.1
---

Every [shape](/docs/shapes) can be moved in any direction by invoking the `move` function with direction. For example, to move a shape named `greeting` to the `RIGHT`, the command we write is

```
greeting.move(RIGHT)
```

![Revine Move Example](https://user-images.githubusercontent.com/4745789/136987897-3c66b590-7604-49d0-86bc-7e22dd63e333.gif)

a general syntax for invoking move is

```
<name of shape>.move(<direction>)
```

## Directions

The available directions in which the shape can be moved are

 - `RIGHT`
 - `LEFT`
 - `UP`
 - `DOWN`

## Example

To continuously move the greeting "Hello" to the right we write

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
