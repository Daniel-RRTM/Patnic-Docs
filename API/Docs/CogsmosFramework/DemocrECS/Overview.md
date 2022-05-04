# DemocrECS  
  
## Introduction
This part of the Framework is responsible to save and declare attributes of game elements.  
  
We are following the basic principles of Data oriented Programming, which does not try to mirror real Situations by Inheritance and Polymorphism, but favors a faster to access and more flexible style of implementations. 
  
---
  
## Structure
  
We use a common variant called ECS, in addition of a Flyweight pattern called Template
**Here is a short summary of the Structure:**

[**E** ntity](../DemocrECS/Entity/Entity.md):  
`` An Object with Hashmaps of Components, overall composing a game element  ``      
    
[**C** omponent](../DemocrECS/Entity-Attributes/Components/Component.md):  
``A container for a value, standardiced by its name ``

[**T** emplat]():  
``A set of components which are commonly shared``
  
[**S** ystem]():  
`` A plugable module of functions which modify, create or delete Entities``
  
---
  
## Personal changes
---
### Proxyfunctions as alternative to variables 
Even simple manipulations on a Component of an entity can take up quite some space:  
````
entity.getComp("C_1_IS_WALKABLE").value = false
````  
Hence why we implemented different [Children for Entities](../DemocrECS/Entity/Entity.md),  
they add for each common anominated Component a function by its name.  
  
Every TileEntity for example, needs the information if you can walk on them.
```
if entity.isWalkable(): getDirection()  
```
---

