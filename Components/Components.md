Components are a piece of code that is used as functionality for the programmer to manipulate when writing the object's code, they can be added and removed.
```java
addComponent(myComponent);
//Some code
removeComponent(myComponent);
```

## Create custom components

To create a component only two requesites must be met, the class must inherit the Engine.Component class, and it might need a constructor, like in the example below:

```java
package pack.pack.pack.Assets.Components;
import pack.pack.pack.Engine.Components;

public class MyCoolComponent extends Component{

	private int myVariable = 1;
	public MyCoolComponent(int myVariable){

		this.myVariable = myVariable;
	}
}
```

You may add any needed methods and those will be called like normal.

## Default engine components

When creating a Himawari2D project the following component's will be automatically added to your project:
* [[Transform]]
* [[Image rendering]]
* [[Collision]]
* [[Animation]]
* [[Physics]]
* Camera

last edited: **24/04/2023**