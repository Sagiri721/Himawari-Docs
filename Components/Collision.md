To establish collision between objects, both the objects that will be colliding, to create a collider the collider bounds will have to be specified, these can be the image size or a custom size.
```java
RectCollider collider = new RectCollider(transform, new Vec2(32, 32));
addComponent(collider);
```

A collider's solidness can be disabled using the _solid_ attribute, to keep an object solid but ignore it's collision with certain objects that belong to certain tags, you may use the _ignoreTag()_ functions, all the tags that are in the ignored tag will not collide with the specific collider.

To check for collisions on command there are various methods that may be used, namely:
* isColliding(), to check if the object is colliding with any other object.
* willCollideWith(Object obj, Vec2 position), to check if given a position the collider would collide with a certain object.
* willCollide(Vec2 position), to check if given a position the collider would collide with any object.
* isCollidingWith(Vec2 point), to check if the object is colliding with a given point.
* isCollidingWith(RectCollider collider), to check if the object is colliding with a given collider.
* getCollisionArea(RectCollider collider), to get the collision area between two different colliders.

last edited: **Sagiri on 24/04/2023**