# tmx2tscn

Convert TMX maps to GodotEngines TSCN so you can use Scenes/Nodes as tiles.

## Usage
0. Download and install Tiled http://www.mapeditor.org
1. Create a new map
  * Orientation: Orthogonal
  * Tile layer format: CSV
  * Tile render order: Right Down
2. Create a tileset: Map > New tileset
3. Add some tiles (If you have chosen "Collection of Images")
4. Click on a tile and at Properties add a new property named "scene" with value "res://dir/scene.tscn" (the location of scene) so a tile would represent a scene.
5. After finishing the map, export it as JSON format.
6. Run "tmx2tscn.py"

## Options
* -i=file.json    : Input file, default: input.json
* -o=file.tscn    : Output file, default: output.tscn
* -oo=true/false  : Origin offset, default: true
* -h              : This help file
