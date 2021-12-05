---
title: Circle
seq: 2.4
---

The `circle` shape draws a circle on the [canvas](/docs/canvas). To draw the circle provide the `center` parameter that specifies the center of the circle, and the `radius` specifying the radius of it.

To understand how to declare and draw a shape please refer, to [this](/docs/shapes) document.

## Example

To declare and draw a circle named `TheBigRedCircle` that is centered at point `(250, 250)` with radius of `100` and thickness of `4` units, filled with [Red](/docs/colors) color we write the following statement.

```
shape TheBigRedCircle(circle):
  .color = BLACK
  .fill = RED
  .center = (250, 250)
  .radius = 100
  .thickness = 4
endshape
```

![Revine Shape Circle](https://user-images.githubusercontent.com/4745789/139802924-4623154a-15ed-4abb-960d-a7a40c7a57fc.png)

## Parameters

| Parameter | Description | Possible values | Default | Required? |
|------------|------------|-----------------|-----------|---------|
| `center`  |  position of the center of the circle | [point](/docs/point) | - |  Yes |
| `radius`  |  radius of the circle | `0` to `500` | - |  Yes  |
| `thickness`  |  the thickness of the circle | `1` to `100` | `2`  |  No  |
| `color`  |  the color of the border | [builtin colors](/docs/colors) | `BLACK`  |  No  |
| `fill`  |  the color to fill the circle with | [builtin colors](/docs/colors) | `WHITE`  |  No  |
