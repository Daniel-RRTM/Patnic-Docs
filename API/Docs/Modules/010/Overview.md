# 010 - ProcGen Actor

### Summary
This module randomly generates an Actor by its limits of its Template and can delete it. 
  
---
### Generall Functions
| <h3 style="width:100px"> **Name** </h3> | <h3>**Return Type**</h3> | <h3 style="width:300px"> **Notation** </h3>                           |  
|---------------------------------------------|--------------------------|-----------------------------------------------------------------------|
| RNGenerateBasicActor(templateIndexString)            | *Dictionary*                   | creates a Dictionary of all needed Infos to instanciate an Actor        |
| createActorTemplate(rNGeneratedActorDict)               | *ActorEntity*                   |Instanciates an Actor by Dictionary (**must have the content from the return of above**) |
| removeActorFromGame(ActorEntity)                | *void*                   | frees ActorEntity when possible |
