# Sound

The Himawari2D framework supports .mp3 and .wav files.
Sound may be added to the engine files via the Sounds folder.

## Instantiate sound object

To create a sound object, you need to pass in the name of the file and if the sound will loop or not.
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

## Audio gain

You can change the audio volume using the static functions _setGlobalGain_ in the followijng way:
```java
Sound.setGlobalGain(-20);
```
The above code will change the volume gain by -20 decibels, making it quieter.
last edited: **Sagiri on 17/04/2023**