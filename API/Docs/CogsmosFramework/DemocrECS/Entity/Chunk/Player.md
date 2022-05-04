### Systems
For readabillity are the many getter nested in proxy-functions, following Functions return their corresponding System:  
* kitsets
* kitparts
* skills
* attributes
* indirects
#
### Kitsets-Functions
| <h3 style="width:100px"> **Name** </h3> | <h3>**Return Type**</h3> | <h3 style="width:300px"> **Notation** </h3>                           |  
|---------------------------------------------|--------------------------|-----------------------------------------------------------------------|
| getAll()                | *Array*                   | returns an array of all KitSetEntities the player is currently able to use |
| getByNr(Integer)                          | *KitSetEntity*                   | returns KitSetEntity corresponding to its Key-input        |
| getByName(String)                          | *KitSetEntity*                   | returns KitSetEntity corresponding to its ``C_12_INDEX_NAME``        |
| remove(KitSetEntity)                          | *void*                   | removes KitSetEntity of the players Inventory (**DOES NOT DISASSEMBLE TO KITPARTS**)        |
| append(KitSetEntity)                          | *void*                   | removes KitSetEntity of the players Inventory (**DOES NOT REMOVEKITPARTS OF TEAM_SHARED LIST**)        |
#
### Kitparts-Functions
| <h3 style="width:100px"> **Name** </h3> | <h3>**Return Type**</h3> | <h3 style="width:300px"> **Notation** </h3>                           |  
|---------------------------------------------|--------------------------|-----------------------------------------------------------------------|
| getAll()                | *Array*                   | returns an array of all KitPartEntities the player is currently able to use |
| getByNr(Integer)                          | *KitPartEntity*                   | returns KitPartEntity corresponding to its Key-input        |
| getByName(String)                          | *KitPartEntity*                   | returns KitPartEntity corresponding to its ``C_12_INDEX_NAME``        |
| remove(KitPartEntity)                          | *void*                   | removes KitPartEntity of the players Inventory (**DOES NOT DISASSEMBLE TO KITPARTS**)        |
| append(KitPartEntity)                          | *void*                   | removes KitPartEntity of the players Inventory (**DOES NOT REMOVEKITPARTS OF TEAM_SHARED LIST**)        |
#
### Skills-Functions
| <h3 style="width:100px"> **Name** </h3> | <h3>**Return Type**</h3> | <h3 style="width:300px"> **Notation** </h3>                           |  
|---------------------------------------------|--------------------------|-----------------------------------------------------------------------|
| crafting()                | *Integer*                   | returns the current competence in this Skill |
| phylosophicing()                | *Integer*                   | returns the current competence in this Skill |
| conceptualication()                | *Integer*                   | returns the current competence in this Skill |
| percieving()                | *Integer*                   | returns the current competence in this Skill |
| assensing()                | *Integer*                   | returns the current competence in this Skill |
| debugging()                | *Integer*                   | returns the current competence in this Skill |
| enduring()                | *Integer*                   | returns the current competence in this Skill |
| coping()                | *Integer*                   | returns the current competence in this Skill |
| filtering()                | *Integer*                   | returns the current competence in this Skill |
| sneaking()                | *Integer*                   | returns the current competence in this Skill |
| repressing()                | *Integer*                   | returns the current competence in this Skill |
| silencing()                | *Integer*                   | returns the current competence in this Skill |
#
### Attributes-Functions
| <h3 style="width:100px"> **Name** </h3> | <h3>**Return Type**</h3> | <h3 style="width:300px"> **Notation** </h3>                           |  
|---------------------------------------------|--------------------------|-----------------------------------------------------------------------|
| logic()                | *Integer*                   | returns the current competence in this attribute |
| agillity()                | *Integer*                   | returns the current competence in this attribute |
| reaction()                | *Integer*                   | returns the current competence in this attribute |
| constitution()                | *Integer*                   | returns the current competence in this attribute |
| strength()                | *Integer*                   | returns the current competence in this attribute |
| intuition()                | *Integer*                   | returns the current competence in this attribute |
| charisma()                | *Integer*                   | returns the current competence in this attribute |
| willpower()                | *Integer*                   | returns the current competence in this attribute |
#
### Indirects-Functions
| <h3 style="width:100px"> **Name** </h3> | <h3>**Return Type**</h3> | <h3 style="width:300px"> **Notation** </h3>                           |  
|---------------------------------------------|--------------------------|-----------------------------------------------------------------------|
| maxKitSlots()                | *Integer*                   | returns the current competence in this calculated value |
| hitpoints()                | *Integer*                   | returns the current competence in this calculated value |
| carriageCapacity()                | *Integer*                   | returns the current competence in this calculated value |
| mentalLimit()                | *Integer*                   | returns the current competence in this calculated value |
| physicalLimit()                | *Integer*                   | returns the current competence in this calculated value |
| socialLimit()                | *Integer*                   | returns the current competence in this calculated value |