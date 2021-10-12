---
title: Move
seq: 3.1
---

The `MOVE` command moves the mentioned [shape](/docs/shapes) in the specified direction.

```
MOVE greeting RIGHT 50
```

## Example

To declare and draw a TEXT shape named `greeting` with text "Hello" at position `(100, 100)` in color [Red](/docs/colors) we write the following statement.

```
SHAPE TEXT
  .name greeting
  .text "Hello"
  .color red
  .x 100
  .y 100
ENDSHAPE
```

![Revine Shape Text](https://user-images.githubusercontent.com/4745789/136927615-725abceb-af4c-4eb6-8431-1ec7ce37a771.gif)

## Parameters

| Parameter | Description | Possible values | Default | Required? |
|------------|------------|-----------------|-----------|---------|
| `name`  |  name of the shape | any text |  |  Yes  |
| `text`  |  text to be drawn | any text |  |  Yes  |
| `color`  |  the color of the text | [builtin colors](/docs/colors) | `BLACK`  |  Yes  |
| `x`  |  x coordinate of the text | `0` to `500` | `0` |  No  |
| `y`  |  y coordinate of the text | `0` to `500` | `0`  |  No  |

> Currently there is no way to change the font or the size.
