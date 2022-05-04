# Atlas for Tiles

## Usage
has as expansion a Hashmap which collects Tiles ordered by its TileSet.

## Functions

### getTileSetEntries()
**Returns :**  All Tiles of a all TileSets as *Hashmap* 

key of each Array of Tiles is the name of TileSet. 
*If you are looking for a single TileSet, the function getEntry(index) may be more suitable.*  

**Example:**  
```
var allTileSets   = API_001_Atlas.Tiles().getTileSetEntries()
var sumOfTileSets = int(allTileSets.size())+1
print("PatnicRoom has "+ str(sumOfTileSets) +" themes/sets for Tiles!")
```  
  
---  
  
### getTilesOfSet(tileSetName)  
**1st Parameter :** name of TileSet as *String*  

**Returns :** All TileEntities in a TileSet as *Array*.  

**Example:**  
```
var tileSetName   = "Terrain"
var allTilesInSet = API_001_Atlas.Tiles().getTilesOfSet(tileSetName)
var sumOfTileSet  = int(allTilesInSet.size())+1
print("The TileSet "+ tileSetName +"has "+ str(sumOfTileSet) +"different Tiles")
```  
  










