To establish collision between objects, both the objects that will be colliding, to create a collider the collider bounds will have to be specified, these can be the image size or a custom size.
```java
RectCollider collider = new RectCollider(transform, new Vec2(32, 32));
addComponent(collider);
```

A collider's solidness can be disabled using the _solid_ attribute, to keep an object solid but ignore it's collision with certain objects that belong to certain tags, you may use the _ignoreTag()_ functions, all the tags that are in the ignored tag will not collide with the specific collider.

last edited: **Sagiri on 17/04/2023**