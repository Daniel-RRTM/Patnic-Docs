# Tiles

## Introduction
Those Entities are detrimental for the Gameworld.  
They are simple enviromental Objects like a patch of grass or concrete, and hold information about the capabillities to interact with them. For example, whether the patch is burnable or not.  
 
---

## Common Components
  
---
### Generall
| <h3 style="width:119px"> **function** </h3> | <h3>**Return type**</h3> | <h3 style="width:150px"> **Component Class-name** </h3> | <h3 style="width:210px"> **Usage** </h3> |  
|-------------|-------------|--------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| [description](../../Entity-Attributes/Components/List/0.md) | String      | C_0_DESCRIPTION      | Lore for Worldbuilding                                                                      |
| [isWalkable](../../Entity-Attributes/Components/List/1.md)  | bool        | C_1_IS_WALKABLE      | Determinds if an ActorEntity can stand on it                                                |
| [textureID](../../Entity-Attributes/Components/List/12.md)   | String      | C_12_ATLAS_INDEX       | Readable variant of the staticTilesetNr, set together by an IFS of ``Tileset_Row_Collumn``  |
| [tileName](../../Entity-Attributes/Components/List/6.md)    | String      | C_6_NAME        | Oneliner reference of max 2 Words                                                           |
| [layer](../../Entity-Attributes/Components/List/3.md)       | String      | C_3_LAYER            | Convention of ``ENUM.SOKRATILES.LAYER`` determining on which layer its percieved            |
  
---
### toStrings
| <h3 style="width:119px"> **function** </h3> | <h3>**Return type**</h3> | <h3 style="width:150px"> **Component Class-name** </h3> | <h3 style="width:210px"> **Usage** </h3> |  
|-------------|-------------|--------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| type | String      | ???      | ???                                                                      |
| mouseHover_quack  | String        | C_6_NAME      | ducktyped function to show name by hovering the mouse over it                                                 |
  
---
### Spacial
| <h3 style="width:119px"> **function** </h3> | <h3>**Return type**</h3> | <h3 style="width:150px"> **Component Class-name** </h3> | <h3 style="width:210px"> **Usage** </h3> |  
|-------------|-------------|--------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| pos | Vector2D      | Instance-variable for perfomance reason      | returns a dictionary-like structure with ``x``  and  ``y`` keys and their float values              |
| poxX  | int        | Instance-variable for perfomance reason      | place on the X-Axis on the Tilemap                                                |
| posY   | int      | Instance-variable for perfomance reason       | place on the Y-Axis on the Tilemap  |
  
---
### Tilemap Parse
| <h3 style="width:119px"> **function** </h3> | <h3>**Return type**</h3> | <h3 style="width:150px"> **Component Class-name** </h3> | <h3 style="width:210px"> **Usage** </h3> |  
|-------------|-------------|--------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| [staticTilesetNr](../../Entity-Attributes/Components/List/7.md) | int      | C_7_STATIC_TILESET_NR      | Number of the Texture in the Tileset Atlas                       |
| [matrixNoise](../../Entity-Attributes/Components/List/5.md)  | int        | C_5_MATRIX_NOISE      | WIP |
| [magicNoise](../../Entity-Attributes/Components/List/4.md)   | int      | C_4_MAGIC_NOISE       | WIP |
  
---
  
  
  