The transform component applies spatial properties to an object, defining it's position, rotation and scale.
Every object has a transform component by default.

## Moving across the screen

To move an object we use it's transform component, there are two different ways to translate an object's position:

```java
//This will move an object 1 pixel to the right ignoring any objects that it may come into contact with
transform.translate(new Vec2(1, 0));
```

```java
//This will move the object 10 pixels to the right, but if the given collider comes into collision with another object, the movement will be canceled
transform.translate(new Vec2(10, 0), (RectCollider) getComponent(RectCollider.class));
```

## Rotating an object

To change an object's rotation, you can use the _Transform.rotate(float)_ method.

```java
//The input should be in degrees and between 0 and 360
transform.rotate(10f);

//When the input overflows the maximum value od 360, the applied rotation will be of value - 360 * n
transform.rotate(380f);
```

Another way to rotate an object in a known direction is using the _Transform.lookAt(Object)_ method, this method will calculate the necessary angle to be facing another object and apply it.

```java
Object target = Object.FindObject("player");
transform.lookAt(target);
```

## Scaling an object

To definine the scale of an object, the setter _Transform.setScale(Vec2)_ may be called:

```java
transform.setScale(new Vec2(2,1));

//Or
transform.setScale(2, 1);
```

last edited: **28/04/2023**