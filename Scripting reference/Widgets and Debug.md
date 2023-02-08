# Widgets and Debug
Widget and Debugging are two classes that can be used to draw primitive graphics to the screen, there is one main difference between these two, Debug take into account the camera's position and draws dynamic graphics, while Widgets are directly drawn to the window.

Widget and Debug have very similar methods, they both can draw:
* Rectangles
* Round rectangles
* Circles
* Ellipses
* Lines
* Text
* Grids
* Sprites
* A health bar

To support different colors, the _setColor_ method can be called, and to fill instead of drawing hollow shapes, the _setDrawType_ method can be called.

```java
Widget.setColor(Color.PINK);
Widget.drawText("Health: " + hp, 10, 10, g);

Widget.setDrawType(Debugging.type.FILLED);
Widget.drawRectangle(new Rectangle(5,5 20, 20), g);

// Vec2 start, Vec2 dimensions, float amount, float maxAmount, Color background, Color borderColor, Color minColor, Color maxColor, Direction direction, boolean border, Graphics2D g
Debugging.drawHealthBar(transform.position, new Vec2(16, 300), hp, 100, Color.BLACK, Color.BLACK, Color.RED, Color.GREEN, Widget.Direction.LEFT, true);
```

last edited: **Sagiri** on **02/02/2023
