---
title: Move
seq: 3.1
---

The `MOVE` command moves a declared [shape](/docs/shapes) in the specified direction by a specified distance. `MOVE` command has the following syntax

```
MOVE <name of the shape> <direction> <distance>
```

For example, to move the [TEXT](/docs/text) object named `greeting` to the `RIGHT` by `50` units, we write

```
MOVE greeting RIGHT 50
```

![Revine Move Example](https://user-images.githubusercontent.com/4745789/136987897-3c66b590-7604-49d0-86bc-7e22dd63e333.gif)

## Directions

The available directions in which the shape can be moved are

 - `RIGHT` or `EAST`
 - `LEFT` or `WEST`
 - `UP` or `NORTH`
 - `DOWN` or `SOUTH`

## Example

To move the greeting "hello" along the square of side `50` units we write

```
SHAPE TEXT
  .name greeting
  .text "Hello"
  .color red
  .position (100, 100)
ENDSHAPE

MOVE greeting RIGHT 50
MOVE greeting UP 50
MOVE greeting LEFT 50
MOVE greeting DOWN 50
```

![Revine Move Text in Square](https://user-images.githubusercontent.com/4745789/136987603-ab76a6f6-779d-448c-aa04-7d8a4c01d877.gif)
