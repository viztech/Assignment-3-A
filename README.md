# Assignment-3-A

This assignment is a rehash of our in-class work in Week 4, and is meant to build your familiarity with arrays, objects, and the basics of drawing in d3. Here, we will try to programatically create a random pattern of circles and squares.

Here are some useful hints, organized step by step.

## Setting up the drawing environment

Review the steps with which we created, and sized, an `svg` drawing environment. The boilerplate is set up for you, but you need to complete one line of code to reflect the margin conventions we covered in class.

## Create an array of data points to generate our random pattern

Instead of a simple array of numbers, here we need to generate an array of `objects`. Attributes of this object (that we need to manually create and randomize) include: x position, y position, size, color, and type (whether circle or square). Eventually, each element of the array should have the form
```
  {
    x: 203, //random between 0 and 'width'
    y: 20, //random between 0 and 'height'
    size: 32, //random between 0 and 50,
    color:rgb(230,89,19),
    type:0
  }
```
HINT: to randomize between circle and square, create a 'type' attribute and use `Math.round()' to set its value to either 0 or 1. 0 could represent circle, 1 square.

## Draw the symbols

Iterate through the array we created using its `.forEach()` method.
