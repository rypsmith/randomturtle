# Turtle moves around LEDs randomly

## Introduction @unplugged

This time you can use the "Turle" extension to have a LED move around the screen on a random path.

![Animation of the initial project.](https://raw.githubusercontent.com/rypsmith/randomturtle/master/randomTurtle.gif)

## Step 1 - Setup

Start by removing the ``||basic:on start||`` block. Keep the ``||basic:on plot||``.

## Step 2 - Make variables

Next go to the ``||variables:Variables||`` category and make a variable called ``||variables:turnDirection||`` 

## Step 3 - set up variable

Place the ``||variables:set turnDirection||`` block in the ``||basic:forever||`` block.

```blocks
let turnDirection = 0
basic.forever(function () {
    turnDirection = 0
})
```

## Step 4 - make it random

Now go and get a ``||math:pick random||`` block and place it inside the ``||variables:set turnDirection||`` block.

```blocks
let turnDirection = 0
basic.forever(function () {
    turnDirection = randint(0, 10)
})
```

## Step 5 - set values

Set the values for the ``||math:pick random||`` to be from 0 to 1. This will act as a true/false or a left/right toggle for our turtle.

```blocks
let turnDirection = 0
basic.forever(function () {
    turnDirection = randint(0, 1)
})
```
