---
title: Rectangle
seq: 2.3
---

The `RECTANGLE` shape draws a rectangle on the [canvas](/docs/canvas). To draw the rectangle provide the parameter `position` that specifies the top-left corner, and `width` and `height` specifying the width and the height of the rectangle respectively. You can optionally specify the `color` and `thickness` of the rectangle and can choose to color `fill` it.

To understand how to declare and draw a shape please refer, to [this](/docs/shapes) document.

## Example

To declare and draw a rectangle named `TheBigRedRectangle` at the point `(100, 100)` with width being `100`, height being `40`, thickness of `2` units, and filled with [Red](/docs/colors) color we write the following statement.

```
SHAPE RECTANGLE
  .position (100, 100)
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
| `position`  |  the position of the top-left corner | [point](/docs/point) | - |  Yes  |
| `width`  |  width of the rectangle | `0` to `500` | - |  Yes  |
| `height`  |  height of the rectangle | `0` to `500` | - |  Yes  |
| `thickness`  |  the thickness of each side | `1` to `100` | `2`  |  No  |
| `color`  |  the color of the side | [builtin colors](/docs/colors) | `BLACK`  |  No  |
| `fill`  |  the color to fill the rectangle with | [builtin colors](/docs/colors) | `WHITE`  |  No  |
| `name`  |  something you want to call this shape | any text | some random text |  No  |
