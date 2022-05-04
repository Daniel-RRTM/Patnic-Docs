# Atlas for KitParts

## Usage
has as expansion a Hashmap which collects Tiles ordered by its TileSet.

## Functions

### sortEntries()
**Returns :**  void

can be used to sort KitParts after some new got added.
Should not be neccessary after Booting the Game.
  
---  
  
### getEntryByName(tileSetName)  
**1st Parameter :** value of ``C_6_NAME`` as *String*  

**Returns :** corresponding KitPart as *child of KitPartEntity*  

can be used if only the name of a kit is known, for example by UI-elements  

**Example:**  
```
var kitPartName = "X_C_1"
var kitPartEnt  = API_001_Atlas.KitParts().getEntryByName(kitPartName)
print(kitPartName +" has a rarity of "+ kitPartEnt.rarity())
```  
  
---  
  
### getKitGroup(string_enum_kitCat)  
**1st Parameter :** name of TileSet as *enum* or its *String*  

**Returns :** all KitPartEntities of the Category   

**Example:**  
```
var allMeeleKits = API_001_Atlas.Tiles().getKitGroup("MEEELE")
var sumOfMeele  = int(allMeeleKits.size())+1
print("there are "+ str(sumOfMeele) +" meele weapons")
```  










