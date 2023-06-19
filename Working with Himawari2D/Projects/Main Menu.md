The main menu of the application consists of six submenus, and some of the functions of these submenus are implemented graphically with button clicks.

1. File
2. Game
3. Code
4. Resource Control
5. Git
6. Settings

The first File menu is the simplest and aims to create an interface with the management application itself. It offers the possibility to close the current project or create an executable file of the project.

The Game menu aims to create an interface between the programmer and the physical game files themselves. This menu allows opening the game's folder and running the game for testing purposes, enabling the programmer to test the code they have written. This operation is done using the compile.bat file created with the project.

The Code menu allows interaction with the code files that the programmer can develop. It allows opening the project's pom.xml, which is essentially the Maven project definition file, and opening the main code file responsible for controlling the game's loading. This menu also allows performing some functions related to the proper functioning of the map editor's graphics. It enables recompiling objects and image references, which respectively remind the program of which objects can be instantiated and remind the map editor of the image associated with each object. These processes are usually performed automatically when needed, but in case of failures, they can also be executed manually through this menu.

The Resource Control menu creates an interface between the programmer and all the multimedia resources inherent to the project they are developing, including images, audio, and fonts. This menu allows copying these resources from any location on the computer to their respective folders within the project. 
![Pasted image 20230608211837.png](../images/Pasted%20image%2020230608211837.png)
It is also with this menu that we can open the project's resource folder if there is a need to add any content manually. The Resource Control menu also allows importing libraries in two ways: through a dependency string or through a library management page loaded from the Himawari2D website. The libraries on this page are added by other users and may be exactly what the programmer is looking for.  
![Pasted image 20230608211905.png](../images/Pasted%20image%2020230608211905.png)

The Git menu provides a graphical interface for version control of the project using Git and GitHub. This menu can easily be replaced by an application like GitHub Desktop, but it is still a convenient addition to have a simple embedded version control within the application. This menu includes the following functionalities:
• Initialize a Git repository
• Set and reset a remote GitHub repository
• Commit all changes made
• Push or pull from the remote repository
• Switch the current branch

The last menu is the Settings menu, which allows defining the executable's metadata, the game's settings, and some of the editor's settings. This menu opens an interface to customize the game's settings, which has three tabs: System, Physics, and Input. The System tab allows changing the application's color scheme, the code editor used when opening a code file, the frame delay of the game, and whether the delta time should be calculated fixedly. The Physics tab allows changing various settings of the physics simulation. Finally, the Input tab allows changing the key mapping used by the Engine.Input.Input.java class.

![Pasted image 20230608212002.png](../images/Pasted%20image%2020230608212002.png)

This menu also allows opening the executable's metadata definition page. These data are stored in the engine-options.json file mentioned in the previous chapter.

![Pasted image 20230608212014.png](../images/Pasted%20image%2020230608212014.png)