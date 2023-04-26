To apply physical properties to your game objects, you may like to use the built-in _Body_ component.
Adding a _Body_ component to an object will make it oblige to forces, like gravity and any other that may be manually applied.

```java
// The heavier the object the more force it will be needed to move it
int mass = 1;

Body body = new Body(transform, collider, mass);
```

To get the current object's acceleration the _Body.calculateAcceleration_ method can be used like so:

```java
float acc = ((Body) object.getComponent(Body.class)).calculateAcceleration();
if(acc < 1){
	//Pretty slow
}else if(acc > 40) {
	//Pretty fast
}
```

## Applying forces

Applying forces to an entity is the most important part of a _RigidBody_ like object, forces can be applied with a 2D vector, the force's strength is defined by the vector magnitude, the longer the vector the stronger the force. 
To apply a force you'll need to call the _Body.ApplyForce(Vec2)_ method like so:

```java
//Make character jump
body.ApplyForce(Vec2.UP.times(10)); 

//Give character knockback
body.ApplyForce(body.totalForce.inverse().times(20));
```

last edited: **26/04/2023**