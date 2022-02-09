---
title: Onkey
seq: 4.1
---

Revine provides a way to interact with keyboard through the `onkey` statement. The statement allows you to add listeners on a certain set of keys - typically all alphabets and define the statements that needs to run when the corresponding key is pressed.

`onkey` statements allows you to fire the movements, actions, animation statements only and they need to be wrapped between `onkey` and `endonkey`. You can define as many `onkey` statements and it enables you to create hyper-interactive artwork and games. The statements  The syntax of using the `onkey` statement is

```
onkey <character>
  ... statements
endonkey
```

To move the text "Hello" up when key `w` is pressed, down when `s` is pressed, left when `a` is pressed, and right when `d` is pressed you would write the following code

```
shape greeting(text):
  .text = "Hello"
  .color = RED
  .position = (100, 100)
endshape

onkey w
  greeting.move(UP)
endonkey

onkey a
  greeting.move(LEFT)
endonkey

onkey s
  greeting.move(DOWN)
endonkey

onkey d
  greeting.move(RIGHT)
endonkey
```

![Revine onkey example](https://user-images.githubusercontent.com/4745789/153281382-3770d022-fbf5-414c-ae6b-41fda54897af.gif)
