# 008 - CLI

### Summary
This module  holds the Collection of the procedures the customiced/hardocoded events which happen with Entities.
  
---
  
### Functions
  
### getGroupedSyntax()
**Returns :**  Dictionary of _009_MetaData

returns all information about all Cmds, they are grouped in commonalities.  
This grouping makes itterating not that comfortable, try getAllCmdMeta() for this.    
  
````
for category in API_008_CLI.getGroupedSyntax().values():
    for cmd in category.values():
        var key         = cmd["input"]
        cmdsSyntax[key] = cmd
        cmdsToString.append(key)
````
  
---  
  
### getMetaByInputKey(key)
**1st Parameter :** String of possible inputs

**Returns :**  Dictionary with all MetaData to this Command

Used as Getter
  
````
getMetaByInputKey(cmd)["class"].run(arrOfParameter)
````
  
---  
  
### getAllCmdMeta()
**Returns :**  Dictionary with direct MetaData as Value, keyed by their input

Used for Itterating through all MetaDatas 
  
````
for entry in API_008_CLI.getAllCmdMeta().values():
    var parameter = entry.parameter as PoolStringArray
    var row = [entry.input,entry.toString,str(parameter.join(", "))]
    if !"WIP" in entry.input: mdWriter.add_row_table(row)
````
  
---  
  