# Geometry
The geometry class utilities provide support for geometrical calculations to be done during runtime.
This class supports:
* Circle geometry;
* Rectangular geometry;
* 2D Vector geometry;

## Vectors

A 2d vector represents a point in 2D space, movement in 2D space or 2D dimensions.
Below is an example of how to instantiate vectors.
```java
//Constant vectors
Vec2 nullVector = Vec2.ZERO;
Vec2 upVector = Vec2.UP;

//Custom vectors
Vec2 myVec = new vec2(25, 5.3f);
myVec.setValues(10, myVec.y);
```
2D vectors support a number of mathematical and logical functions, namely: sum, subtraction, multiplication, division, absolute vector, invert, magnitude and value clamping.

![vectors](images/vectors.png)

## Rectangles & Circles

A rectangle is a shape that can be instantiated with it's x and y positions, followed by their width and height. Circles need an x and y position followed by a radius.
```java
Rectangle rect = new Rectangle(50, 50, 200, 30);
Circle circle = new Circle(rect.x, rect.y, 30);
```
Both of these support the basic Shape interface functions.
The **Contains** and the **Intersects**.

![shapes](images/shapes.png)

last edited: **10/01/2023**