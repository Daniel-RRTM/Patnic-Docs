# KitPart

## Introduction
KitParts are the single buildingblocks for [KitSets](KitSet.md).   
  
---
  
## Types

###### Core
The most Important. It **defines** its Description and its use!   
Therefore its **Mandatory** for every Kit!  
It also **determinds possible Upgrades**!

###### Upgrade
The Improvement. It **specialices** the Kit in a certain of aspect!   
This part is **optional**!  
It may **debuff other aspects** in some rare cases!

###### Trait
A passive Benefit. It gives a small **generall advantage** under conditions!    
This part is **optional**!  
**needs to be on same plane**, is independant of the Core!
  
---
  
## Common Components
  
#### General  
| <h3 style="width:119px"> **function** </h3> | <h3>**Return**</h3> | <h3 style="width:200px"> **Usage** </h3> | <h3 style="width:160px"> **Notation** </h3> |  
|------------------|---------|----------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| [index](../../Entity-Attributes/Components/List.md#C_12_ATLAS_INDEX)            |  String  | fluff and lore shown in onlook-action                    | recommended length is 40 characters at max                                                    |
| [name](../../Entity-Attributes/Components/List.md#C_6_NAME)         | String  | oneliner reference                                       | recommended length is 2 words at max                                                          |
| [description](../../Entity-Attributes/Components/List.md#C_0_DESCRIPTION)  | Integer | index number of corresponding Texture                    | not recommended for freqeunt use.   please use textureID for improved readabillity.           |  
    
---
   
#### Categories  
| <h3 style="width:119px"> **function** </h3> | <h3>**Return**</h3> | <h3 style="width:200px"> **Usage** </h3> | <h3 style="width:160px"> **Notation** </h3> |  
|------------------|---------|----------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| [mType](../../Entity-Attributes/Components/List.md#C_37_M_TYPE)            |  String  | fluff and lore shown in onlook-action                    | recommended length is 40 characters at max                                                    |
| [catType](../../Entity-Attributes/Components/List.md#C_31_KIT_CAT_TYPE)         | String  | oneliner reference                                       | recommended length is 2 words at max                                                          |
| [partType](../../Entity-Attributes/Components/List.md#C_38_KIT_PART_TYPE)  | Integer | index number of corresponding Texture                    | not recommended for freqeunt use.   please use textureID for improved readabillity.           |  
| [family](../../Entity-Attributes/Components/List.md#C_69_KITSET_FAMILY)  | Integer | index number of corresponding Texture                    | not recommended for freqeunt use.   please use textureID for improved readabillity.           |  
    
---
   
#### ToString  
| <h3 style="width:119px"> **function** </h3> | <h3>**Return**</h3> | <h3 style="width:200px"> **Usage** </h3> | <h3 style="width:160px"> **Notation** </h3> |  
|------------------|---------|----------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| [mechanicalSummary](../../Entity-Attributes/Components/List.md#C_35_KIT_MECHANICAL_SUMMARY)            |  String  | fluff and lore shown in onlook-action                    | recommended length is 40 characters at max                                                    |
| [modTime](../../Entity-Attributes/Components/List.md#C_36_KIT_MOD_TIME)         | String  | oneliner reference                                       | recommended length is 2 words at max                                                          |
| [cooldownTime](../../Entity-Attributes/Components/List.md#C_33_COOLDOWN_TIMER)  | Integer | index number of corresponding Texture                    | not recommended for freqeunt use.   please use textureID for improved readabillity.           |  
      
---

#### Usage  
| <h3 style="width:119px"> **function** </h3> | <h3>**Return**</h3> | <h3 style="width:200px"> **Usage** </h3> | <h3 style="width:160px"> **Notation** </h3> |  
|------------------|---------|----------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| [rarity](../../Entity-Attributes/Components/List.md#C_48_RARITY)            |  String  | fluff and lore shown in onlook-action                    | recommended length is 40 characters at max                                                    |
| [event](../../Entity-Attributes/Components/List.md#C_49_EVENT_REFERENCE)         | String  | oneliner reference                                       | recommended length is 2 words at max                                                          |
        
---