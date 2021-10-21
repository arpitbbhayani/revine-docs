---
title: Line
seq: 2.2
---

The `LINE` shape draws a line between two points on the [canvas](/docs/canvas). You can optionally specify the color to be used while drawling the line.

To understand how to declare and draw a shape please refer, to [this](/docs/shapes) document.

## Example

To declare and draw a LINE shape named `TheBigRedLine` between the points `(100, 100)` and `(200, 200)` in color [Red](/docs/colors) we write the following statement.

```
SHAPE LINE
  .name TheBigRedLine
  .x1 100
  .y1 100
  .x2 200
  .y2 200
  .color red
  .width 2
ENDSHAPE
```

![Revine Shape Line](https://user-images.githubusercontent.com/4745789/137705081-94474c75-5474-41ea-b61c-1a81b68f9e98.gif)

## Parameters

| Parameter | Description | Possible values | Default | Required? |
|------------|------------|-----------------|-----------|---------|
| `name`  |  name of the shape | any text |  |  Yes  |
| `x1`  |  x coordinate of the first point P1 | `0` to `500` | `0` |  No  |
| `y1`  |  y coordinate of the first point P1 | `0` to `500` | `0` |  No  |
| `x2`  |  x coordinate of the first point P2 | `0` to `500` | `0` |  No  |
| `y2`  |  y coordinate of the first point P2 | `0` to `500` | `0` |  No  |
| `color`  |  the color of the line | [builtin colors](/docs/colors) | `BLACK`  |  No  |
| `width`  |  the width of the line | `1` to `30` | `2`  |  No  |

> Currently there is no way to change the width of the line.
