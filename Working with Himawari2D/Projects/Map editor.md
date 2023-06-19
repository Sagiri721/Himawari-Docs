The map editor is one of the main components of the entire graphical interface. It was also the first component to be developed. This component allows dynamic editing of rooms, enabling the creation of background patterns and the insertion of dynamic and adjustable objects. To create a map, you need some data. A map requires a tileset and tile size. A tileset is simply an image, and the tile size determines how many pixels the fragments of the original image should be cut into. After the image is cut, each individual piece can be placed in the room to create meaningful patterns. Lastly, a room needs a size, and the larger the room, the more tiles can be placed.

The map editor is divided into three distinct tabs: editing tools, object parameters, and editor tools. The editing tools tab is the most populated with functions and contains the tools that are essential to the room editing experience.

![Pasted image 20230608212432.png](../images/Pasted%20image%2020230608212432.png)

The first button, represented by a Yoshi icon, is the tile selector. It allows the programmer who is editing the map to choose one of the tiles that were cut when the map was created. After selecting a tile, it can be effectively placed on the map with a left click. These tiles can be placed in one of four methods:

1. One-by-one: One click equals one tile.
2. Line: The mouse can be dragged to draw tiles.
3. Rectangle: A rectangle is drawn when the mouse is dragged.
4. Fill: A section of identical tiles is replaced by a new tile that was selected.

![Pasted image 20230608212513.png](../images/Pasted%20image%2020230608212513.png)

The application also consists of three layers. Tiles will only be drawn if the drawing layer is selected. The other two layers are the object layer, which allows the creation, deletion, and visualization of objects, and the editing layer, which allows the editing of data for previously placed objects. The layers are represented respectively by a grass block, sand, and brick.

O segundo botão da interface, represented by a Lakitu image, allows the creation of an object to be placed on the map. An object can be defined with several properties, including its name, which should correspond to the Java file name of the object in the code, its rotation, and its scale. Once the properties of an object are defined, it can be placed on the map with a left-click when the second layer is selected. If no image is associated with the placed object, it will be represented as illustrated in Figure 101. However, when a project is imported, the actual sprites can be used for a more realistic map representation. An object can be deleted with a right-click, and it can be inspected with a middle-click.

The third and fourth buttons are similar, both displaying an image of a question mark block. The first button defines the zoom level of the window. When clicked, it presents the user with a dialogue asking for the window size in tiles. This button can also be replaced by using the mouse wheel, which automatically zooms using the same technique. The second button defines the camera position. By setting a higher x position than the current one, all objects will move to the left, and it becomes possible to see tiles and objects that were previously not visible. This functionality can also be achieved using the "H," "J," "K," and "L" keys, as well as the arrow keys. The label "root point" indicates the current position of the camera.

The fifth and sixth buttons modify the graphical settings of the editor itself. When the rainbow-colored star is pressed, the zoom and position settings are reset. When the green pipe is pressed, the grid overlay is disabled, allowing the map to be observed as it will be presented in the game.

The seventh and eighth buttons are two very important buttons, represented respectively by a red mushroom and a green mushroom. The first button exports all the information defined in this editing session to a map folder in the previously demystified format. The second button imports a previously exported map to the current workspace, allowing for reediting. Once a map is exported, it can be saved with each change.

The last two buttons are represented by an image of Mario and a Goomba. The first button presents the programmer with a list of all placed objects and their information. The second button only works when the editing layer is selected. The editing layer allows the programmer to select objects and edit their properties such as rotation and position. When this layer is selected and the last button of the interface is pressed, it is possible to select a parent for the selected object.

The second tab of the editor is named "object parameters" and only works when either the editor is being opened by the project manager or when objects are manually imported through the third tab, which will be mentioned shortly. This second tab allows the programmer to define objects dynamically to be placed on the map. Manually typing the name of each object can lead to consistency errors, and rewriting the properties of each object whenever a different object needs to be placed can be tedious. Therefore, this tab allows for dynamic and error-free definition of objects for the map.

![Pasted image 20230608212543.png](../images/Pasted%20image%2020230608212543.png)

Using the arrow on the right side of the text box allows you to iterate through the objects associated with the current project. On the other side of the menu, there are text boxes to define the scale and rotation of each object. Any changes made in this menu are applied in real-time.

Finally, we have the "Editor Tools" tab, which contains a total of four buttons with useful tools for the map editing application.

![Pasted image 20230608212551.png](../images/Pasted%20image%2020230608212551.png)

The "Import Tileset" button allows you to redefine the tileset to be used for the current room. Clicking this button allows you to select a new tileset for the currently edited room.

The "Import Objects" button allows you to switch the list of objects to be used in the second tab. This enables you to import a different set of objects for the map being edited.

The "Save project" button allows you to save the map information in case it has already been exported or imported. This action can be quickly performed by pressing the "S" key.

Lastly, the "Shortcuts" button opens an image that serves as a guide, helping the programmer understand how to quickly use the editor.

![Pasted image 20230608212556.png](../images/Pasted%20image%2020230608212556.png)