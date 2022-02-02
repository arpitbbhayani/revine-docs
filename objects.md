---
title: Objects
seq: 1.3
---

Multiple [shapes](/docs/shapes) can be combined to create an object. The object can then be animated or interacted with as a singular entity rather than individual shapes. For example, a cloud (shown below) is composed of 5 overlapping [circles](/docs/circle); and hence we can create an object named `cloud` consisting of 5 shapes of type [circle](/docs/circle).

![Cloud Object Disintegration](https://user-images.githubusercontent.com/4745789/145831221-17ca480d-2178-4097-aa53-cffe70394f7a.png)

## Create an Object

To create and draw any object on the [canvas](/docs/canvas), declare and draw it using the `object` statement. Declaration of a
shape involves

 - specifying the name of the object
 - specifying the shapes that would create this object
 - ending the declaration using `endobject`

```
object <name of shape>():

  shape <somename>(<type>):
    .<property2> = value2
    .<property3> = value3
  endshape

  shape <somename>(<type>):
    .<property2> = value2
    .<property3> = value3
  endshape
  
  ...

endshape
```

> Note, you can wrap any number and types of shapes within an object and you will find information about the properties supported by a shape in the documentation of that shape.

Once an object is defined you can animate the object by using its name. To understand it in detail, check the example below.

## Example

In this example, we animate create a cloud and make it go left and right, as shown below

![Revine Cloud Animation](https://user-images.githubusercontent.com/4745789/140464897-4a0ff9c4-08b7-4178-9b57-1e1a84b5391f.gif)

We see that a cloud is made up of 5 overlapping circles and hence we first create `5` shapes of type circles of varied radii.

```
shape c1(circle):
  .center = (100, 200)
  .radius = 75
  .color = lightgrey
  .fill = lightgrey
endshape

shape c2(circle):
  .center = (170, 170)
  .radius = 125
  .color = lightgrey
  .fill = lightgrey
endshape

shape c3(circle):
  .center = (270, 160)
  .radius = 145
  .color = lightgrey
  .fill = lightgrey
endshape

shape c4(circle):
  .center = (330, 180)
  .radius = 100
  .color = lightgrey
  .fill = lightgrey
endshape

shape c5(circle):
  .center = (380, 200)
  .radius = 75
  .color = lightgrey
  .fill = lightgrey
endshape
```

When we run above snippet of code, we get a cloud.

![Revine Cloud](https://user-images.githubusercontent.com/4745789/145835053-8cf81892-5858-4dad-a287-64422b42abba.png)

Now that we have the desired object, we wrap it up in [Object](/docs/objects) declaration and name it `cloud` as shown below. We have just wrapped the 5 shapes between `object cloud():` and `endobject`. This groups the 5 circles and create an object named `cloud`.

```
object cloud():

  shape c1(circle):
    .center = (100, 200)
    .radius = 75
    .color = lightgrey
    .fill = lightgrey
  endshape

  shape c2(circle):
    .center = (170, 170)
    .radius = 125
    .color = lightgrey
    .fill = lightgrey
  endshape

  shape c3(circle):
    .center = (270, 160)
    .radius = 145
    .color = lightgrey
    .fill = lightgrey
  endshape

  shape c4(circle):
    .center = (330, 180)
    .radius = 100
    .color = lightgrey
    .fill = lightgrey
  endshape

  shape c5(circle):
    .center = (380, 200)
    .radius = 75
    .color = lightgrey
    .fill = lightgrey
  endshape

endobject
```

Now that we have a `cloud`, making it go right is simple. we simply invoke the [move](/docs/move) command as shown below

```
loop
  cloud.move(RIGHT)
endloop
```

The above commands will move `cloud` to the right. The complete example can be seen in the [showcase](https://revine.arpitbhayani.me/showcase/cloud).
