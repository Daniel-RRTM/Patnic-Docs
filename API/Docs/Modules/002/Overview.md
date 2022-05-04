# 002 - Tilemap_Structure

## Usage
Expansion of [SokraTiles](../../CogsmosFramework/SokraTiles/Overview.md), its used for getters which are either not dependant on a Layer or in need of Multiple Ones.   
Its also where the instanciated Classes fpr each Layer are located.
  
---
  
## Systems
  
| Name                | Usage                                             |
|---------------------|---------------------------------------------------|
| [Layer_Actor_NPC](NPC.md)                | functions for Layer                        |
| [Layer_Actor_Player](Player.md)        | functions for Layer |
| [Layer_Animation_Condition](Condition.md)               | functions for Layer         |
| [Layer_Animation_Selection](Selection.md)             | functions for Layer                   |
| [Layer_Matrix_Floor](Matrix_Floor.md)           | functions for Layer          |
| [Layer_Matrix_Interactables](Matrix_Interactable.md)    | functions for Layer time          |
| [Layer_Meat_Floor](Meat_Floor.md)    | functions for Layer          |
| [Layer_Meat_Interactables](Meat_Interactable.md)              | functions for Layer                |
| [Layer_Magic_Floor](MagicFloor.md)              | functions for Layer                |
| [Layer_Magic_Interactables](MagicInteractable.md)              | functions for Layer KitParts                |
| TileInterpreter  | runs contextual events when stepping on them(can be called via this API)             |
| Utils     | Helpers for other Systems                     |

  
---
  

## Functions
  
### getMovePos(startingPos,directionFourEnum)
**1st Parameter :** Vector2 of starting-position  
**2nd Parameter :** int of [ENUM.DIRECTION_FOUR](../../Conventions/Enums.md#DIRECTION_FOUR)

**Returns       :** Vector2D
  
calculates the Vector when walked one time in a direction
  
**Example:**  
```

``` 
  
---
  
### getMovePosByMultiple(startingPos,directionFourEnum,times)
**1st Parameter :** Vector2 of starting-position  
**2nd Parameter :** Integer of [ENUM.DIRECTION_FOUR](../../Conventions/Enums.md#DIRECTION_FOUR)  
**3rd Parameter :** Integere of times walked 

**Returns       :** Vector2D
  
calculates the Vector when walked X time in a direction
  
**Example:**  
```

``` 
  
---
  
### interpreteTile(entity,chunkToInterprete)
**1st Parameter :** Entity which walked 
**2nd Parameter :** System which should be used to interprete the walk by

**Returns       :**  Dynamic  
  
triggers events when Actors walk on Tilemap.  
I.E possibilty to enter Rest when walking on the PanicRoom.  
I.E attaching burning to an Actor when walking into it.
  

**Example:**  
```

``` 
  
---



