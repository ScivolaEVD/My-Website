# Code Block

# Python Code

```python

import random
from turtle import Turtle

def recursive_circles(turtle, angle, quantity, delta, radius):
    colors = ["red", "orange", "brown", "green", "blue", "purple"]
    color = random.choice(colors)
    turtle.color(color)
    turtle.right(angle)
    turtle.forward(delta)
    unit_angle = 360.0/quantity
    for x in range(quantity):
        turtle.circle(radius)
        turtle.left(unit_angle)
    radius = radius - delta
    if (radius > 7):
        recursive_circles2(turtle, angle, quantity, delta, radius)

def main():
    ANIMATION_SPEED = 0
    mikey = Turtle()
    mikey.speed(ANIMATION_SPEED)
    recursive_circles(mikey, 20, 20, 5, 100)

main()

```

[return to home page](./README.md)
