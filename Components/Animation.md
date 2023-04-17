# Create animation from sprite sheet
To create an animation the first step is to get the sprite sheet of the animation, that is, a big picture that contains every frame. In the current framework version 1.0.3, multiple line sprite sheets are not supported.
Example of a sprite sheet:
![spritesheet](miniwalk.png)

This type of image is interpreted as an array of buffered images.
The animation data type stores all the frames of a sprite sheet, to create an animation use the static method: _[Sprite](Sprites.md).createAnimation_
```java
Sprite image = new Sprite("mini idle.png");
Animation walk = Sprite.createAnimation(image, 64, 64, 0, 0, true);
```
This method takes as parameters the full sprite sheet, the width of an individual sprite, it's height, the x position from where to start cropping, the y position from where to start cropping, and a boolean value, which is true if the sprites are spread out horizontally, and false in the case they were spread out vertically.

# Initialize animator component
The animator component takes an array of animations and controls what the _ImageRenderer_ component displays, the image renderer must also be given.
```java
Animation idle = Sprite.createAnimation( new Sprite(bimg), 64, 64, 0, 0, true);
Animation walk = Sprite.createAnimation(new Sprite(bimg2), 64, 64, 0, 0, true);
Animation[] anims = {idle, walk};

Animator animator = new Animator(anims, renderer);

addComponent(animator);
```
Animations may be added programmatically by calling the _Animator.addAnimation_ function which adds a different animation to the Set. Each animation is assigned an ID which corresponds to the order in which they were added to the animations Set.
To play an animation the _Animator.play_ function must be called:
```java
animator.play(0, 0);
```
In the above example, the "idle" animation will be played, as it was the first to be added to the array, as for the second parameter, it asks for the starting frame of the animation, it should be zero in most cases but it may be changed as needed.
In opposition, _Animator.pause_ will stop the animation from playing.

Some parameters that can be messed around with are the _imageIndex_ and _imageSpeed_, which control respectively the current animation frame, and the play speed.

```java
animator.imageSpeed = 0.01f; //fast
animator.imageSpeed = 3f; //slow
```

last edited: **Sagiri on 13/10/2022**