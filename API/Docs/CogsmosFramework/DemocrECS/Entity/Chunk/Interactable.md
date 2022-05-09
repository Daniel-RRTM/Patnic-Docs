# Interactables

## Introduction
Those Entities are in between Tiles and Actors.

Much like Tiles, they are static and can not change their position on the Tilemap. But they are able to be part of a greater narrative, just like Actors.  
Actors can usually not walk on Interactables and are reactionary. 
  
---
    
## Common Components
  
---
#### General
| <h3 style="width:119px"> **function** </h3> | <h3>**Type**</h3> | <h3 style="width:200px"> **Usage** </h3> | <h3 style="width:160px"> **Notation** </h3> |  
|------------------|---------|-------------------------------------------------|-----------------------------------------------------------------------------------------------|
| [description](../../Entity-Attributes/Components/List/0.md)      | String  | fluff and lore shown in onlook-action           | recommended length is 40 characters at max                                                    |
| [textureID](../../Entity-Attributes/Components/List/12.md)        | String  | toString() of staticTilesetNR                   | is a convention of 3 fields with "_" as IFS:<br>  ``Tileset_Row_Collumn``                     |
| [layer](../../Entity-Attributes/Components/List/37.md)            | Integer | name of layer where its mapped                  | convention of ``ENUM.SOKRATILES_LAYER.``X``_GROUND``<br> X for ``MEAT`` ``MATRIX`` ``MAGIC``  |
| [tileName](../../Entity-Attributes/Components/List/6.md)         | String  | oneliner reference                              | recommended length is 2 words at max                                                          |
| [staticTilesetNR](../../Entity-Attributes/Components/List/7.md)  | Integer | index number of corresponding Texture           | not recommended for freqeunt use.   please use textureID for improved readabillity.           |  
  
---
#### Spacial
| <h3 style="width:119px"> **function** </h3> | <h3>**Type**</h3> | <h3 style="width:200px"> **Usage** </h3> | <h3 style="width:160px"> **Notation** </h3> |   
|------------------|---------|-------------------------------------------------|-----------------------------------------------------------------------------------------------|
| type             | ENUM    | identifier to differenciate from other entities | convention of ``ENUM.TYPES_ON_MAP.TILE``                                                      |
| [isWalkable](../../Entity-Attributes/Components/List/1.md)       | BOOLEAN | Determinds if Actors can stand on Tile          |                                                                                               |
| mouseHover_quack | String  | duck-typed proxy-function to show on Mousehover |                                                                                               |
| pos              | Vector2 | position of Entity on x and y on Tilemap        | posX and posY can be for single getter. <br>  Are Converted from Double to Integer!           |  
  
---
#### Influencial
| <h3 style="width:119px"> **function** </h3> | <h3>**Type**</h3> | <h3 style="width:200px"> **Usage** </h3> | <h3 style="width:160px"> **Notation** </h3> |  
|------------------|---------|-------------------------------------------------|-----------------------------------------------------------------------------------------------|
| [matrixNoise](../../Entity-Attributes/Components/List/5.md)      | Integer | negative modifier for sourrunding Electronics   | WIP                                                                                           |
| [magicNoise](../../Entity-Attributes/Components/List/4.md)       | Integer | negative modifier for sourrunding Magics        | WIP                                                                                           |
  
---   
  
  
  