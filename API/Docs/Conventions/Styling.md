### Introduction
Our Code may be from a professionell buissness point of view lengthy, spacy, too much or even useless commenting and unconventional.  
  
We are aware of Conventions like PEP 8 or CCG. Buit there are good reasons why we dont use them:
1. **Experimental Design**: We often try new Ideas and patterns just for the fun and learning of it, see fast-prototyping.  
2. **Interdisciplinary**: PatnicRoom is set together by 5 different Repos with different script-languages.
3. **Its open ended**: There is no Definition of Done for our Project. With each new update, a intuitive Navigation becomes more beneficial.
4. **We are Hobbyist**: Everything is free of charge, therefore we sometimes have to compromise between our limited time and ressources and best practices.  
  
---
  
### General

We are using **GD-Script**, even though Godot support C#.  
no need to sweat, its quite **beginnerfriendly** and on its surface similar to **Python**.  
(Note: we may use C# for perfomance-heavy things in the Future)

  
---
  
### Example for Sub-System 
Context:   
Parsing a multi-leveled TileMap(100x100) with multiple percievable layers, converting the Map-specific UID into instanciated Counterparts.
````
extends Object
class_name _SokraTiles_TileMapParser

static func parseTileMap(filepathToMap:String) -> Dictionary:
  #>>> Sanitication <<<#
  var mapMetaData = _getRelevantMetaData(filepathToMap)
  var parsedMap   : Array

  
  #>>> Itterating each Layer each Heights <<<#
  for heightLevel in mapMetaData.levels:
    var parsedLevel : Dictionary
    for currentPerception in heightLevel.keys():
      var content = heightLevel.currentPerception


      #>>> Formatting of Layer by Context <<<
      var formatedPerception: Dictionary
      if    "PLAYER"   in currentPerception :   formatedPerception = _findPlayer(content)
      elif  "INTERACT" in currentPerception :   formatedPerception = _categoriceInteracts(content)
      elif !currentLayer.empty()            :   formatedPerception = _parseDefaultLayer(mapMetaData,content)
      

      #>>> Validating <<<#
      if !formatedPerception.empty(): parsedLevel[currentPerception] = formatedPerception
      else: printerr("!!ERROR!! at Parsing Tilemap in "+filepathToMap+" at Layer "+currentPerception)   
    parsedMap.append(parsedLevel)
      
  return parsedMap



static func _getRelevantMetaData(tiledImport:String) -> Dictionary:
  var tiledImport = Util.JSONParser.fileToDictionary(filepathToMap)
  var mapMetaData : Dictionary

	mapMetaData["size"]    = Vector2(tiledImport.height, tiledImport.width)
	mapMetaData["levels"]  = getLayersOfLevel(tiledImport.layers)
	mapMetaData["tileNrs"] = tiledImport.tilesets.size()
	return mapMetaData
````
  


### Example for API 
Context:  
Simple Class to collect and return a Template of each TileEntity in the Game.
````
extends Object
class_name DemokrECTS_Atlas


var _entryComponentRef : Dictionary    # VAR [entry.indexComponent.value] : [Array of all Comp.name]   
var _EntriesOfAtlas    : Dictionary    # VAR [indexComponent.value] : [Instance of Entity]             
var _classOfEntries                    # VAR needs typing by SubAtlas (I.E. TileEntity)                


  
# ----- GETTER --------------------------------------------------------------- ##


# FUNC returns ALL, use getEntry() for specific            
# FUNC Dict uses [indexComponent] : [Instance of Entity]   
func getEntries() -> Dictionary: 
	return _EntriesOfAtlas 


# FUNC index is value of C_12_ATLAS_INDEX   
# FUNC return is type-casted as Entity      
func getEntry(index:String) -> Entity: 
	return _EntriesOfAtlas[index] as Entity


# FUNC searchedTerm is dynamic typed   
func getEntriesWithCompValue(searchedTerm,compname:String) -> Array:
	var validEnts : Array
	for entry in getEntriesWithComp(compname):
		if entry.getCompValue(compname) == searchedTerm : validEnts.append(entry) 
	return validEnts



# ----- SETTER --------------------------------------------------------------- ##


func addEntity(ent,compIndex="C_12_ATLAS_INDEX"):
	if ent is _classOfEntries:
		if !_EntriesOfAtlas.has(ent):
			var index                 = ent.getCompValue(compIndex)
			_EntriesOfAtlas[index]    = ent
			_entryComponentRef[index] = ent.components.keys()
		
		else: printerr("Error in Atlas_TileEntity! ["+str(ent.name())+"] already exists")
	else: printerr("Error in Atlas_TileEntity! ["+(ent.name())+"] could not be added")
````


### Further Reading

###### Typing 
We use as much **Static Typing** as possible.

###### Duck-typing  
We are using ducktyped functions as workaround for Interfaces.  
We mark them By ending them with ``_quack()``
unfortunately Godot does not support abstract classes

###### Capitalication  
* Variables have CamelCase  
* NodeNames have PascalCase
* Classes have NameOfApiInPascal_SubsystemInPascal  
* Enums have SCREAM_CASE
* Conventionsaliced Lists of Classes have SCREAM_CASE (I.E Components)

###### Encapsulation  
local functions and variables begin with an underscore (``_``).
Godot does not support private, hence this workaround.

###### Node-References  
We recommend to use onready and static typing if possible and to reference it via absolute path, I.E :  
``onready var nameOfNode : Panel = get_node("/root/MainMenue/Selection/Backgorund")``   
If you want to Itterate through your Nodes (I.E Inventories) we recommend to put them into a VBoxContainer and naming them after numbers counting upwards






