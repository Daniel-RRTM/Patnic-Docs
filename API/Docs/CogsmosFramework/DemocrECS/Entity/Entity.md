# Entities

## Introduction
Entities are a pillar in our gamedesign, almost every Item, Actor or obstacle can be tracked back to this class.  
broken down,they are just a collection of diffrent lists which contains the defining values of the game-element and references to other Entities which are in some relation to them. 
    
---  
  
## Entity Attributes
### [Components](../Entity-Attributes/Components/Component.md)
Lorem Ipsum  

### [Templates](Template.md)
Lorem Ipsum  

### [Flags](../Entity-Attributes/Flags/List.md)
Lorem Ipsum  

### [Properties](../Entity-Attributes/Properties/List.md)
Lorem Ipsum  

### [Conditions](../Entity-Attributes/Conditions/List.md)
Lorem Ipsum  
  
---  
  
## Children with improved functioncalls
  
| Class                   | Context                                           |
|-------------------------|---------------------------------------------------|
| [Tile](../Chunk/Tile)                | Floor of the current Chunk                        |
| [Interactable](../Chunk/Interactable)        | More complex inanimated Objects,standing on Tiles |
| [Actor](../Chunk/Actor)               | NPC with their own will, gear and actions         |
| [KitPart](../KitSet/KitPart)             | One of the 3 Parts of an KitSet                   |
| [Condition](../Event/Condition)           | Manipulates an affected Entity over time          |
| [KitSet](../KitSet/KitSet)              | Usable Abillity merged by KitParts                |
  
---
  
## Functions
* getComp(compIndex)
* getCompValue(compIndex)
* addComponent(Component)
* removeComponent(compIndex)
* hasComponent(compIndex)

* getCompTemp(tempIndex,compIndex)
* getCompTempValue(tempIndex,compIndex)
* addTemplate(tempIndex,Template)

* addFlag(enumNumber)
* removeFlag(enumNumber)
* hasFlag(enumNr)

* addProperty(enumNumber)
* removeProperty(enumNumber)
* hasProperty(enumNumber)

* hasCond(condIndex)
  
---  
  
## Common Functions

### getComp(compIndex)
**1st Parameter :** [String of class of Component](../Component/List.md)

**Returns       :** Class of the same Name  

Can be used to get the Documentation of a Component or to change its instanced Value.  
Components and Entities dont have a setter-function, because we want in DOP/ECS the manipulation of Data only happening in Systems.
  

**Example:**  
```
var ent = API_001_Atlas.Tile.getEntry("Terrain_0_0") 
for compToString in ent.components.keys(): 
    print(ent.getComp(compToString).getAutoDoc().nameToShow) 
```  
  
---  
  
### getCompValue(compIndex)
**1st Parameter :** [String of class of Component](../Component/List.md)

**Returns :**  Component.value as dynamically typed

The probably most used Function! returns the instanced Value of a Component of an Entity.  
Can only be used to read and not write due to reference by value (one above).  
  
Note:  
Its dynamic typing may cause some trouble, for exmaple by trying to print out a int typed value of an Component. We are aware of it and fix it soon.
  

**Example:**  
```
for currentTile in API_001_Atlas.Tile.getEntries(): 

    # is allready a String, no crashing
    var toPrint = currentTile.getCompValue("C_6_NAME")+" "  
    
    # to prevent crashing because of boolean return
    if currentTile.getCompValue("C_1_IS_WALKABLE") :   toPrint += "is walkable"
    else                                           :   toPrint += "is not walkable"
    
    print(toPrint) 
```  
  
---  
  
### getCompTemp(tempIndex,compIndex) 
WIP   
  
---  
  
### getCompTempValue(tempIndex,compIndex)
WIP
  
---
  
### addComponent(compInstance)
**1st Parameter :**   [Instance of a Component](../Component/List.md)

**Returns :**  void

adds the instance into the ``components`` Dictionary of the Entity with its name as a Key.  
Its name is always instanciated as its classname, hence each entity can have no Component twice.  
Instanciating Components always need a vlaue in its Constructor, in the most Cases both are happening in the same Line.
  

**Example:**  
```
var allEnts : Array

for name in ["Hello","World"]:
    var ent = Entity.new()
    ent.addComponent(C_6_NAME.new(name))
    allEnts.append(ent)

for ent in allEnts :  print(ent.getCompValue("C_6_NAME"))
```  
   
---
  
### removeComponent(compName)
**1st Parameter :**   [Stringof class of Component](../Component/List.md)

**Returns :**  void

erases the entry form ``components`` Dictionary.  
This does not free the instance, just erases the reference!
  

**Example:**  
```
for currentTile in API_001_Atlas.Tile.getEntries():
    currentTile.removeComponent("C_12_ATLAS_INDEX")
    print("no more TileMaps!!!")
```  
  
---
  
### addTemplate(tempIndex,compIndex)
WIP   
  
---
  
### addFlag(flagName)
**1st Parameter :** name of Flag in String

**Returns :**  void

adds a marker to the entity, use hasFLag() to validate.  
Note: its still the ToString of the enum, we are aware of that and will fix it
  

**Example:**  
```
Lorem Ipsum
Dolor Emit  
```  
  
---

### removeFlag(tempIndex)
**1st Parameter :**  
**2nd Parameter :**  

**Returns :**  

Lorem Ipsum
Dolor Emit  
  

**Example:**  
```
Lorem Ipsum
Dolor Emit  
```  
  
---
  
### addProperty(tempIndex)
**1st Parameter :**  
**2nd Parameter :**  

**Returns :**  

Lorem Ipsum
Dolor Emit  
  

**Example:**  
```
Lorem Ipsum
Dolor Emit  
```  
  
---
  
### removeProperty(tempIndex)
**1st Parameter :**  
**2nd Parameter :**  

**Returns :**  

Lorem Ipsum
Dolor Emit  
  

**Example:**  
```
Lorem Ipsum
Dolor Emit  
```  
  
---
  
### hasProperty(tempIndex)
**1st Parameter :**  
**2nd Parameter :**  

**Returns :**  

Lorem Ipsum
Dolor Emit  
  

**Example:**  
```
Lorem Ipsum
Dolor Emit  
```  
  
---
  
### hasFlag(tempIndex)
**1st Parameter :**  
**2nd Parameter :**  

**Returns :**  

Lorem Ipsum
Dolor Emit  
  

**Example:**  
```
Lorem Ipsum
Dolor Emit  
```  
  
---
  
### hasComponent(tempIndex)
**1st Parameter :**  
**2nd Parameter :**  

**Returns :**  

Lorem Ipsum
Dolor Emit  
  

**Example:**  
```
Lorem Ipsum
Dolor Emit  
```  
  
---
  
### hasCond(tempIndex)
**1st Parameter :**  
**2nd Parameter :**  

**Returns :**  

Lorem Ipsum
Dolor Emit  
  

**Example:**  
```
Lorem Ipsum
Dolor Emit  
```  
  
---
  



