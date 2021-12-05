---
title: Text
seq: 2.1
---

The `text` shape draws any text/string on the [canvas](/docs/canvas) at the [position](/docs/point) specified in the parameters.

> The font used to render the text is the default one and cannot be changed at the moment. Like the text font, the size of the text is also a constant and cannot be changed.

To understand how to declare and draw a shape please refer, to [this](/docs/shapes) document.

## Example

To declare and draw a `text` shape named `greeting` with text "Hello" at position `(100, 100)` in color [RED](/docs/colors) we write the following statement.

```
shape greeting(text):
  .text = "Hello"
  .color = RED
  .position = (100, 100)
endshape
```

![Revine Shape Text](https://user-images.githubusercontent.com/4745789/136927615-725abceb-af4c-4eb6-8431-1ec7ce37a771.gif)

## Parameters

| Parameter | Description | Possible values | Default | Required? |
|------------|------------|-----------------|-----------|---------|
| `text`  |  text to be drawn | any text | - |  Yes  |
| `position`  |  the position at which the text is to be drawn | [point](/docs/point) | - |  Yes  |
| `color`  |  the color of the text | [builtin colors](/docs/colors) | `BLACK`  |  No  |

> Currently there is no way to change the font or the size.
