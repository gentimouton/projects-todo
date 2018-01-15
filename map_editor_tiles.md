
there's multiple parts to it
- **tileset**, eg a PNG of [6x8 tiles of 32x32 px](https://opengameart.org/content/terrain-transitions)). Pixel art. May come with a manifest specifying tile size in px, tile names, or properties about tile corners or edges. Simpler without manifest though.
- **map format**, eg [TMX](http://doc.mapeditor.org/en/latest/reference/tmx-map-format/). Constrains what a "map" is (square vs hexagonal grid, layers, what tile from the tileset goes where, which tile is walkable).
- **map loader**, eg [PyTMX](https://github.com/bitcraft/PyTMX) and [Mr Figs' loader](https://github.com/joereynolds/Mr-Figs/blob/master/src/level_editor.py). Understands map format. Outputs a python object.
- **map renderer**, eg via pygame or pyglet from the object output by the loader.
- **map saver**, converts python object to a file in map format.
- **map editor**, eg [Tiled Map Editor](http://www.mapeditor.org/). Includes a map loader, renderer, and saver. Can have convenience tools like brush and templates. Ultimately, these tools don't get saved into the map, since the format typically does not allow for them.

thoughts
- scripts in maps: it's a spectrum, from Ragnarok (maps have no scripts; scripts live in other files, on top of maps) to all-in-one (scripts live on tiles). For games like Bomberman where tiles and items have few well-defined behaviors, maps could be levels, ie they store items and triggers as well. For games with more diverse behaviors (eg patrols or triggers based on game state), something closer to Ragnarok is the way to go.
