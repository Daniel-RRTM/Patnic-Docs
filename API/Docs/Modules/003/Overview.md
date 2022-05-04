# 003 - Player

### Summary
This module is for getting and manipulating the data of the current Character on the tilemap like Healthpoints or Kitsets and the data shared between his team like kitparts.  
  
---
  
## Functions

### Rest

### getStations()
**Returns :**  All three Stations and their current state.    

contains Information for manipulating KitSets (I.E. current time till completion)
  
**Example:**  
```

```  
  
---  
  
### getCurrentStationSetter()
**Returns :**  Helper function with with corresponding station as reference     

has functions to its Station values (I.E. decrementing time till completion) 
  
**Example:**  
```

```  
  
---  
  


### Player generation 

### getEntries(dictToGenerate)
**1st Parameter :**  Dictionary with Vlaues of Components to Generate Entity  

**Returns :**  Lorem Ipsum  

Lorem Ipsum
  
**Example:**  
```

```  
  
---  
  
### loadQuickStartChar()

**Returns :**  Void  

Generates PlayerEntity of SaveState ``Quickstart`` for special Bootmodes like starting in Panic
  
**Example:**  
```

```  
  
---  
  
### loadCharBySaveStateName(name)
**1st Parameter :**  String of Name of SaveState to generate  
  
**Returns :**  Void  

Generates PlayerEntity of SaveState with that name and sets Runner 1 as currentChar
  
**Example:**  
```

```  
  
---  
  
### setIndirectStats(entity)
**1st Parameter :**  Actor which should get calculated stats  
  
**Returns :**  Void  

Calculates indirect stats (I.E. Hitpoints) of an Actor and adds them as a Component
  
**Example:**  
```

```  
  
---  
  