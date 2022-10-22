### Introduction
Cogsmos is our Framework which keeps the Core-Gameloop together!  
  
Their are separated from Modules for a Number of Reasons:
1. They are dependand on each other, Separation is by their nature very difficult.
2. They one of the first things that need to be initialiced at booting the Game.
3. They usable for all Modules, and not just one specific Game-System



### Parts

| Singleton               | Use                                             |
|-------------------------|-------------------------------------------------|
| [DemocrECS](DemocrECS/Overview.md)           | ECS for Data orientated Programming             |
| [SokraTiles](SokkraTiles/Overview.md)          | Parsing of Tilemap and its Content              |
| [ALECandria](ALECandria/Overview.md)          | Parsing and instanciating external GameData     |
| [AresProcGenes](ArisProcGenes/Overview.md)       | Procedurally generating Chunks, Actors and Loot |
  
  
**Fufact**:  
Its Naming is a play on Wods:   
of "Cog" (on each other relaying pieces of a machine,greater than its sum)  
and "Cosmos" (used in Ancient Greece to describe universal Laws/ abstract Theories).  
  
hence why the Parts are named after Philosophers, each one has something with its Singleton in common 





