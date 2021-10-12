---
title: Shapes
seq: 1.2
---

Every object you draw on [canvas](/docs/canvas) is called a _Shape_. The shape could be a line, a circle, or even text. There are predefined shapes available for you to use and animate in your artwork.

![Revine Shapes](https://user-images.githubusercontent.com/4745789/136773370-d7d3f6e2-4a27-42e6-9644-e05690ff0d17.png)

## Drawing a Shape

To draw any shape on the [canvas](/docs/canvas), declare and draw it using the `SHAPE` statement. Declaration of a
shape involves

 - specifying the type of the shape
 - specifying the properties of the shape
 - ending the declaration using `ENDSHAPE`

```
SHAPE <TYPE OF SHAPE>
  .<property1> value1
  .<property2> value2
  .<property3> value3
ENDSHAPE
```

There are a lot of prebuilt shapes like [TEXT](/docs/text), [CIRCLE](/docs/circle), and [LINE](/docs/line) that
you can use for your animation and artwork. You can find all the supported shapes in the menu on the left-hand side.

Every shape type has a set of properties, like `color`, `name`, `x`, and `y`, that it requires during declaration.
These properties determine how the `TEXT` shape will be rendered on the canvas. The property of the shape always
starts with a `.` followed by the value(s) required for it. Some properties are common across shapes, but every
shape will have a few properties unique to it.

> You will find information about the properties supported by a shape in the documentation of that shape.

Once you have specified the properties, you must specify the end of your shape declaration by putting in an `ENDSHAPE`.

## Example

To draw some text on the canvas, we use the shape [TEXT](/docs/text) and declare it as

```
SHAPE TEXT
  .name greeting
  .text "Hello"
  .color red
  .x 100
  .y 100
ENDSHAPE
```

The above set of statements declare a shape of type `TEXT`, and we have named it `greeting`. The name of the shape should be unique
because it will help us refer this very shape when we animate it. This shape will write the text `"Hello"` on the canvas in color [Red](/docs/colors) at location `(100, 100)`.

You can find more details and supported properties by the `TEXT` shape [here](/docs/text); and similar to this, you can find
other shapes and their supported properties through their corresponding documentation.
