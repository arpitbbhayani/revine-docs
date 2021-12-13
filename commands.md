---
title: Commands
seq: 1.4
---

_Commands_ allow us to interact with the [canvas](/docs/canvas) and the [shapes](/docs/shapes) we drew on it. Every command will take in some parameters required by it to take the necessary actions.

To invoke a command on a shape, just invoke the corresponding function with the necessary arguments. For example, to [move](/docs/move) a shape named `greeting` to the `RIGHT` by `50` units, the command we write is

```
greeting.move(RIGHT, 50)
```

![Revine Command Example](https://user-images.githubusercontent.com/4745789/136987897-3c66b590-7604-49d0-86bc-7e22dd63e333.gif)

The parameters and their order are important, and they depend on the command we fire. The parameters of each command are documented under the corresponding command doc. You can find all the supported commands in the menu on the left-hand side.
