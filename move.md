---
title: Move
seq: 3.1
---

Every [shape](/docs/shapes) can be moved in any direction by invoking the `move` function with arguments - direction and offset. For example, to move a shape named `greeting` to the `RIGHT` by `50` units, the command we write is

```
greeting.move(RIGHT, 50)
```

![Revine Move Example](https://user-images.githubusercontent.com/4745789/136987897-3c66b590-7604-49d0-86bc-7e22dd63e333.gif)

a general syntax for invoking move is

```
<name of shape>.move(<direction>, <offset>)
```

## Directions

The available directions in which the shape can be moved are

 - `RIGHT`
 - `LEFT`
 - `UP`
 - `DOWN`

## Example

To move the greeting "hello" along the square of side `50` units we write

```
shape greeting(text):
  .text = "Hello"
  .color = RED
  .position = (100, 100)
endshape

greeting.move(RIGHT, 50)
greeting.move(UP, 50)
greeting.move(LEFT, 50)
greeting.move(DOWN, 50)
```

![Revine Move Text in Square](https://user-images.githubusercontent.com/4745789/136987603-ab76a6f6-779d-448c-aa04-7d8a4c01d877.gif)
