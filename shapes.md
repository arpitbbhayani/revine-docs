---
title: Shapes
seq: 1.2
---

The most elementary thing that you draw on the [canvas](/docs/canvas) is called a _Shape_. The shape could be a [line](/docs/line), a [rectangle](/docs/rectangle), a [circle](/docs/circle), or even [text](/docs/text).

![Revine Shapes](https://user-images.githubusercontent.com/4745789/136773370-d7d3f6e2-4a27-42e6-9644-e05690ff0d17.png)

## Drawing a Shape

To draw any shape on the [canvas](/docs/canvas), declare and draw it using the `shape` statement. Declaration of a
shape involves

 - specifying the type of the shape
 - specifying the properties of the shape
 - ending the declaration using `endshape`

```
shape <name of shape>(<type>):
  .<property1> = value1
  .<property2> = value2
  .<property3> = value3
endshape
```

There are a lot of built-in shapes like [text](/docs/text), [line](/docs/line), and [circle](/docs/circle) that
you can use for your animation and artwork. You can find all the supported shapes in the menu on the left-hand side.

Every shape type has a set of properties, like `color`, `name`, `position`, that it requires during declaration.
These properties determine how the shape will be rendered on the canvas. Some properties are common across shapes, but every
shape will have a few properties unique to it.

> You will find information about the properties supported by a shape in the documentation of that shape.

Once you have specified the properties, you must specify the end of your shape declaration by putting in an `endshape`.

## Example

To draw some text on the canvas, we use the shape [text](/docs/text) and declare it as

```
shape greeting(text):
  .text = "Hello"
  .color = RED
  .position = (100, 100)
endshape
```

The above set of statements declare and draw a shape named `greeting` of type `text` at position `(100, 100)` in color `RED`.

You can find more details and supported properties by the `text` shape [here](/docs/text); and similar to this, you can find
other shapes and their supported properties through their corresponding documentation.
