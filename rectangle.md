---
title: Rectangle
seq: 2.3
---

The `RECTANGLE` shape draws a rectangle on the [canvas](/docs/canvas). To draw the rectangle provide the parameter `x`, `y` that specifies the top-left corner of the rectangle, and `width` and `height` denoting the width and the height of the rectangle. You can optionally specify the `color`, `thickness` of the rectangle and can choose to `fill` it with a specific color.

To understand how to declare and draw a shape please refer, to [this](/docs/shapes) document.

## Example

To declare and draw a `RECTANGLE` shape named `TheBigRedRectangle` at the point `(100, 100)` with width being `100`, height being `40`, each side being `2` units thick, and filled with [Red](/docs/colors) color we write the following statement.

```
SHAPE RECTANGLE
  .x 100
  .y 100
  .width 100
  .height 40
  .thickness 2
  .color black
  .fill red
  .name TheBigRedRectangle
ENDSHAPE
```

![Revine Shape Rectangle](https://user-images.githubusercontent.com/4745789/138922362-6bb06d44-35ce-4685-b23f-69d11e496657.png)

## Parameters

| Parameter | Description | Possible values | Default | Required? |
|------------|------------|-----------------|-----------|---------|
| `x`  |  x coordinate of the top-left point | `0` to `500` | - |  Yes  |
| `y`  |  y coordinate of the top-left point | `0` to `500` | - |  Yes |
| `width`  |  width of the rectangle | `0` to `500` | - |  Yes  |
| `height`  |  height of the rectangle | `0` to `500` | - |  Yes  |
| `thickness`  |  the thickness of each side | `1` to `100` | `2`  |  No  |
| `color`  |  the color of the side | [builtin colors](/docs/colors) | `BLACK`  |  No  |
| `fill`  |  the color to fill the rectangle with | [builtin colors](/docs/colors) | `WHITE`  |  No  |
| `name`  |  something you want to call this shape | any text | some random text |  No  |
