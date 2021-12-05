---
title: Line
seq: 2.2
---

The `line` shape draws a line between two [points](/docs/points) on the [canvas](/docs/canvas). You can optionally specify the color to be used while drawling the line.

To understand how to declare and draw a shape please refer, to [this](/docs/shapes) document.

## Example

To declare and draw a LINE shape named `TheBigRedLine` between the points `(100, 100)` and `(200, 200)` in color [Red](/docs/colors) we write the following statement.

```
shape TheBigRedLine(line):
  .point1 = (100, 100)
  .point2 = (200, 200)
  .thickness = 2
  .color = RED
endshape
```

![Revine Shape Line](https://user-images.githubusercontent.com/4745789/137705081-94474c75-5474-41ea-b61c-1a81b68f9e98.gif)

## Parameters

| Parameter | Description | Possible values | Default | Required? |
|------------|------------|-----------------|-----------|---------|
| `point1`  |  starting point of the line | [point](/docs/point) | - |  Yes  |
| `point2`  |  ending point of the line | [point](/docs/point) | - |  Yes  |
| `thickness`  |  the thickness of the line | `1` to `100` | `2`  |  No  |
| `color`  |  the color of the line | [builtin colors](/docs/colors) | `BLACK`  |  No  |
