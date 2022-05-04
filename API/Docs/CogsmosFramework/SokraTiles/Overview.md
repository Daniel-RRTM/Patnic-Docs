## Introduction
This part of the Framework is responsible for parsing Tilemaps and Organicing it Managers of each Layer.



## Functions  
  
### Gettign Layer Nodes
you can use **getLayerNode(layerEnum)** to get each Layer of the Tilemap, we suggest to use its proxies for readabillity:  
  
| Function            | Class it returns                      |
|---------------------|---------------------------------------|
| getPlayer()         | SokraTiles_Chunk_Player               |
| getActor()          | SokraTiles_Chunk_Actors               |
| getSelection()      | Sokratiles_Chunk_Selection            |
| getCondition()      | Sokratiles_Chunk_Condition            |
| getMeatInteract()   | SokraTiles_Chunk_Meat_Interactables   |
| getMeatFloor()      | SokraTiles_Chunk_Meat_Floor           |
| getMagicInteract()  | SokraTiles_Chunk_Matrix_Interactables |
| getMagicFloor()     | SokraTiles_Chunk_Matrix_Floor         |
| getMatrixInteract() | SokraTiles_Chunk_Magic_Interactables  |
| getMatrixFloor()    | SokraTiles_Chunk_Magic_Floor          |
  
---  
  
### parseTileMap(filepath)
**1st Parameter :** Filepath to the in Tiled! designed Tilemap as String

**Returns :** Void

Make surue your Tilemap contains of Layers with its M-Type and Entity, like in the Template of ``/GameData/Tiled/TileMaps/Unique/Template.json``
  

**Example:**  
```
generateQUickStartChar()
SokraTiles.parseTilemap("res://Config/experimental tilemap.json")
get_tree().change_scene("res://Src/scenes/Gameloop/PanicMode/PanicMode.tscn")
```  
  
---  
  
### getCompValue(layerEnum,TileMapNode)
**1st Parameter :** enum of its corresponding Layer
**2nd Parameter :** Node of the Manager of the Layer

**Returns :**  Void

Will be initialiced when Scene of Panic-mode enters the tree
  

**Example:**  
```
func _ready():
	.initialice(ENUM.SOKRATILES.LAYER.CONDITION)
	Signals.connect("Actor_Turn_Finished",self,"updateMap")
```  
  
---  
  

  
