# Conditions

## Introduction
Conditions provide a longterm influence for affected entities, the include a functions which is called every start of a round.  
  
---
  
## Attributes

####  affectedEnt : Entity
is a reference to the Entity which is manipulated, it can be attached by ``API_006_Condition.attachConditionToEnt(ent,condIndex,duration,level)`` for more click [here](../../../../Modules/006/Overview.md).  
Its type-castet as Entity   
  
####  effect : Array  
contains the contextual strings for each [effect](Effect.md) that manipulates the Entity

####  level : Integer  
Intensity of the effects, may be not neccessary

####  duration : Integer  
Nuber of rounds to run the effects
  
---
  
## Common Componenets  
| <h3 style="width:119px"> **function** </h3> | <h3>**Return**</h3> | <h3 style="width:200px"> **Usage** </h3> | <h3 style="width:160px"> **Notation** </h3> |  
|------------------|---------|----------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| [index](../../Entity-Attributes/Components/List/12.md)            |  String  | fluff and lore shown in onlook-action                    | recommended length is 40 characters at max                                                    |
| [use](../../Entity-Attributes/Components/List/72.md)         | String  | oneliner reference                                       | recommended length is 2 words at max                                                          |
| [texture](../../Entity-Attributes/Components/List/12.md)  | Integer | index number of corresponding Texture                    | not recommended for freqeunt use.   please use textureID for improved readabillity.           |  
| [name](../../Entity-Attributes/Components/List/6.md)          | String  | RNG-selected lore name of ``Race`` ``Role`` ``Spcialty`` |                                                                                               |
| [by](../../Entity-Attributes/Components/List/71.md)          | String  | RNG-selected lore name of ``Race`` ``Role`` ``Spcialty`` |                                                                                               |
| [description](../../Entity-Attributes/Components/List/0.md)          | String  | RNG-selected lore name of ``Race`` ``Role`` ``Spcialty`` |                                                                                               |
  



