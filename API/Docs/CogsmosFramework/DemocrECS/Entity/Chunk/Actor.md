# Actors

## Introduction
Those Entities are the important kickstarter for Excitement.

Actors are aware beings like humans, but also Animals, Critters, Ghosts or Plants.  
The big difference to Interactables is,Actors follow a goals, initiate events like shooting,  
while Interactables stay reactionary.    
  
---
  
  
  
## Generation
Actors are set togeteher by those three parts which can be procedurallly selected for "random" generation
  
| <h3 style="width:200px"> **Component-name** </h3>          | <h3 style="width:400px"> **Usage** </h3>                                 |  
|------------------------------------------------------------|--------------------------------------------------------------------------|  
| [Races](Atlas/races.md)                                    | Determinds max of Attributes and their Basevalue, also comes with feats  |    
| [Roles](Atlas/roles.md)                                    | Gives a large amount of Skillpoints and some for Attributes              |  
| [Specialties](Atlas/specialties.md)                        | Gives Gear, some little feats and some Skillpoints                       |  
   
--- 
  
  
  
# Unique Functions
  
### mouseHover_quack()
**Returns :**  String

A duck-typed function for all Entities that are present on the Tilemap, it returns a Component-value (here: [Synonym](../../Entity-Attributes/Components/List.md#C_47_SYNONYM)). I.E. used in onLook
  
---
  
  
  
## Component Getter  

---
#### General  
| <h3 style="width:119px"> **function** </h3> | <h3>**Return**</h3> | <h3 style="width:200px"> **Usage** </h3> | <h3 style="width:160px"> **Notation** </h3> |  
|------------------|---------|----------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| [index](../../Entity-Attributes/Components/List/12.md)            |  String  | fluff and lore shown in onlook-action                    | recommended length is 40 characters at max                                                    |
| [name](../../Entity-Attributes/Components/List/6.md)         | String  | oneliner reference                                       | recommended length is 2 words at max                                                          |
| [staticTilesetNR](../../Entity-Attributes/Components/List/7.md)  | Integer | index number of corresponding Texture                    | not recommended for freqeunt use.   please use textureID for improved readabillity.           |  
| [Synonym](../../Entity-Attributes/Components/List/47.md)          | String  | RNG-selected lore name of ``Race`` ``Role`` ``Spcialty`` |                                                                                               |
| description      | String  | fluff and lore shown in onlook-action                    | recommended length is 40 characters at max                                                    |
  
---
   
---
#### Spacial
| <h3 style="width:119px"> **function** </h3> | <h3>**Type**</h3> | <h3 style="width:200px"> **Usage** </h3> | <h3 style="width:160px"> **Notation** </h3> |   
|------------------|---------|-------------------------------------------------|-----------------------------------------------------------------------------------------------|
| type             | ENUM    | identifier to differenciate from other entities | [ENUM.TYPES_._ON_MAP](../../../../Conventions/Enums#TYPES_ON_MAP)                                                     |
| isWalkable       | BOOLEAN | Determinds if Actors can stand on Tile          |                                                                                               |
| mouseHover_quack | String  | duck-typed proxy-function to show on Mousehover |                                                                                               |
| pos              | Vector2 | position of Entity on x and y on Tilemap        | posX and posY can be for single getter. <br>  Are Converted from Double to Integer!           |  

---  
#### Attributes    
| <h3 style="width:119px"> **function** </h3> | <h3>**Type**</h3> | <h3 style="width:200px"> **Usage** </h3> | <h3 style="width:160px"> **Notation** </h3> |  
|------------------|---------|-------------------------------------------------|-----------------------------------------------------------------------------------------------|
| constitution     | Integer | Health, CarriageCapacity                        | physical                                                                                      |
| reaction         | Integer |                                                 | physical                                                                                      |
| strength         | Integer |                                                 | physical                                                                                      |
| agillity         | Integer |                                                 | physical                                                                                      |
| willpower        | Integer |                                                 | mental                                                                                        |
| logic            | Integer |                                                 | mental                                                                                        |
| charisma         | Integer |                                                 | mental                                                                                        |
| intuition        | Integer |                                                 | mental                                                                                        |

---  
#### indirect stats
| <h3 style="width:119px"> **function** </h3> | <h3>**Type**</h3> | <h3 style="width:200px"> **Usage** </h3> | <h3 style="width:160px"> **Notation** </h3> |  
|------------------|---------|-------------------------------------------------|-----------------------------------------------------------------------------------------------|
| carriageCapacity | Integer | kg of gear actor can carry                      |                                                                                               |
| hitpoints        | Integer | Live of Actor                                   |                                                                                               |
| physicalLimit    | Integer |max successes in Dicerole for physical           |                                                                                               |
| mentalLimit      | Integer |max successes in Dicerole for mental             |                                                                                               |
| socialLimit      | Integer |max successes in Dicerole for social             |                                                                                               |
 
  
  