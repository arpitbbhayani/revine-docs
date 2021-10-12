---
title: Commands
seq: 1.3
---

_Commands_ allow us to interact with the [canvas](/docs/canvas) and the [shapes](/docs/shapes) we drew on it. Every command will take in some parameters required by it to take the necessary actions.

For example, the [MOVE](/docs/move) command takes in the following parameters:

 - the name of the shape to be moved
 - the direction of movement
 - the distance to be covered

To move a shape named `hello` in the `RIGHT` direction by `50` units, the command we write is

```
MOVE hello RIGHT 50
```

![Revine Command Example](https://user-images.githubusercontent.com/4745789/136777488-4e2bd63e-889e-41cf-af7c-59f88e0a4aa8.gif)

The parameters and their order are important, and they depend on the command we fire. The parameters of each command are documented under the corresponding command doc. You can find all the supported commands in the menu on the left-hand side.
