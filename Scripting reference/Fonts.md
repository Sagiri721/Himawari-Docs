# Fonts
## True type fonts

True type fonts are fonts that come from a font file like OTF, WOFF, TTF etc...
To intialize a true type font you'll only need the name of the file and the size of the font, like shown bellow:
```java
Font font = new Font("Verdana.ttf", 15);
```

## Image fonts

Image fonts are fonts that come from a tileset like following:
![[tile 1.png]]

To initialize an image font you will need a FontMap object, a start x and start y position, a boolean flag and the order of the characters.
The example bellow is a representation of how to turn the image above int an image font.
```java
TileSet tileset = new TileSet(new Sprite("tiles.png"), 16,16);
FontMap map = new FontMap("abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ", tileset);

Font font = new Font(0, 0, true, map);
```