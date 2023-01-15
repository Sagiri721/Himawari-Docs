# Sound

The Himawari2D framework supports .mp3 and .wav files.
Sound my be added to the engine files via the Sounds folder.

## Instantiate sound object

To create a sound object you need to pass in the name of the file and if the sound will loop or not.
```java
Sound sound = new Sound("mysong.wav", true);
```

## Playing sound

To play sound, you only need to call the play method, and to stop it, just call the stop method.
```java
Sound sound;
@Override
public void Start(){

	sound = new Sound("mysong.wav", true);
	sound.play();
}

@Override
public void Update(float deltaTime) {

	if(Input.mousePressed(0)){
		sound.stop();
	}
}
```

last edited: **Sagiri on 29/11/2022**