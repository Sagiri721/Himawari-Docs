# Input
Receiving input from the user is rather simple, you can get stuff like the position of the mouse, keyboard presses, and automatically calculate movement axis.

## Mouse input
To have mouse input you can use the function _Input.mousePressed_
The mouse buttons are represented by numbers:

* 0 -> Mouse button left;
* 1 -> Mouse button middle;
* 2 -> Mouse button right;

```java
if(Input.mousePressed(0)){
	//Do stuff
}
```

## Keyboard input
To get keyboard input from the user the _Input.isKeyPressed_ function must be called, it receives data from the Keys format, an enumerator with all the keys supported by the engine.

```java
if(Input.isKeyPressed(Keys.Z)){
	//Perform action
}
```

### Movement Axis
Movement axis are variables that can be accessed and whose values vary from only -1 to 1, being -1 when the left value is pressed, 1 when the righ value is pressed and 0 when none are pressed.

These axis can be defined and used for whatever purpouse the programmer sees fit.
The default are:

AxisX | AxisY
------ | ------
A -> D   | W -> S
LEFT -> RIGHT   | UP -> DOWN

These values may be adjusted in the project settings.

```java
Vec2 movement = new Vec2(Input.axisX, Input.axisY);
```

last edited: **Sagiri on 09/12/2022**