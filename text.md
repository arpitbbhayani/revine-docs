---
title: Text
seq: 2.1
---

The `TEXT` shape draws the mentioned text on the [canvas](/docs/canvas) at the position specified by the additional parameters.

The font used to render the text is the default one and cannot be changed at the moment. Like the text font, the size of the text is also a constant and cannot be changed.  

To understand how to declare and draw a shape please refer, to [this](/docs/shapes) document.

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
