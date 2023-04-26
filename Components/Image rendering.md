Image rendering can be achieved with an ImageRenderer component.
To create an Image Renderer you'll need a _Sprite_ and an _Object_.
A sprite can be initialized with the name of the image file.

```java
Sprite myImg = new Sprite("image.png");
ImageRenderer renderer = new ImageRenderer(image, this);

addComponent(renderer);
```

To hide an object the _visible_ property may be edited with the _ImageRenderer.setVisible(boolean)_ function.

An image renderer has 3 properties that can be tweaked, the flipX, flipY and alpha property, these represent respectively the images horizontal mirroring, the vertical mirroring and the image's opacity.

```java
renderer.flipX();
if(!renderer.isFlippedY) renderer.flipY();

// Value from 0 to 1
renderer.setAlpha(0.5f);
```

An image renderer sprite can also be scaled if the image file is too large / small.

```java
renderer.scaleSprite(
	64 /* Width in pixels */, 
	64 /* Height in pixels */, 
	ImageRenderer.scaleAlgorithm.SMOOTH
);
```

last edited: **24/04/2023**