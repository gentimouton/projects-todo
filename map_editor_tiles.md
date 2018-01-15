
there's multiple parts to it
- **tileset**, eg a PNG of [6x8 tiles of 32x32 px](https://opengameart.org/content/terrain-transitions)). Pixel art.
- **map format**, eg [TMX](http://doc.mapeditor.org/en/latest/reference/tmx-map-format/). Constrains what a "map" is (square vs hexa grid, layers, what tile from the tileset goes where, which tile is walkable).
- **map loader**, eg [PyTMX](https://github.com/bitcraft/PyTMX). Understands map format. Outputs a python object.
- **map renderer**, eg via pygame or pyglet from the object output by the loader.
- **map saver**, converts python object to a file in map format.
- **map editor**, eg [Tiled Map Editor](http://www.mapeditor.org/). Includes a map loader, renderer, and saver. Can have convenience tools like brush and templates and such. Ultimately, these tools don't get saved into the map, since the format typically does not allow for them.

