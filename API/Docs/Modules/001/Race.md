This System has no further functions than the common ones:

## Common Functions

### getEntries()
**Returns :**  Hashmap all collected Entities in.  

key of each Entity is the value of Component ``C_12_ATLAS_INDEX``.  
*If you are looking for a single entity, the function getEntry(index) may be more suitable.*  

**Example:**  
```
var allTileEnts = API_001_Atlas.Tiles().getEntries()
var sumOfTiles  = int(allTileEnts.size())+1
print("PatnicRoom has "+ str(sumOfTiles) +" possible tiles!")
```  
  
---  
  
### getEntry(index)  
**1st Parameter :** value of ``C_12_ATLAS_INDEX`` as *String*  

**Returns :** Entity with its corresponding index.  

can be used to instanciates a exact copy of an Element, keep in mind that changing its manipulating Components will greatly influence future procedural generations.  

**Example:**  
```
var tileEnt   = API_001_Atlas.Tiles().getEntry("Terrain_0_0")
var nameOfEnt = tileEnt.name()
print("one of its Tiles is called "+ nameEnt +"!")
```  
  
---  
  
### getEntriesWithComp(compName)  
**1st Parameter :** class-name of Component as *String*

**Returns :** Array of Entities which contain Component

can be used to granulate search for sppecific.
*If you are looking for a specific value, the function getEntriesWithCompValue(searchValue, compName) may be more suitable.*  

**Example:**  
```
var killableTiles  = API_001_Atlas.Tiles().getEntriesWithComp("C_57_HITPOINTS")
var sumOfkillables = int(killableTiles.size())+1
print(str(sumOfTiles) +"Tiles even can be damaged!")
```  
  
---  
  
### getEntriesWithCompValue(searchValue, compName)  
**1st Parameter :** class-name of Component as *String*  
**2nd Parameter :** value of Component as *dynamic* type  

**Returns :** Array of Entities which contain Component and equals searched value

May lead to Performance issues if used in frequently called functions like _process() or _input()

**Example:**  
```
var walkableTiles = API_001_Atlas.Tiles().getEntriesWithCompValue(true,"C_1_IS_WALKABLE")
var sumOfTiles    = int(killableTiles.size())+1
print(str(sumOfTiles) +"Tiles can be stand on!")
```  
  
---
  
### addEntity(Entity)  
**1st Parameter :** Entity, specific child if possibly

**Returns :** void 

Adds Entity into System, prints error if it already exists or has wrong Class.  
Should not be neccessary after Booting the Game.