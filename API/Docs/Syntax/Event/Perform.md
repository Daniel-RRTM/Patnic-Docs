# Perform

### COMP
1. ``FILE``
2. ``COMP``
3. [Component](../../CogsmosFramework/DemocrECS/Entity-Attributes/Components/List.md)  
4. ``SET`` ``INCREMENT BYT`` ``DECREMENT BY``
5. Value  

````
FILE ---> COMP C_1_IS_WALKABLE SET TRUE
FILE ---> COMP C_1_IS_WALKABLE SET FALSE

FILE ---> COMP C_48_RARITY INCREMENT BY 2
FILE ---> COMP C_48_RARITY DECREMENT BY 5
FILE ---> COMP C_48_RARITY DECREMENT SET 1
````
  
---
  


### COND 
1. ``FILE``
2. ``COND``
3. [Condition](../../CogsmosFramework/DemocrECS/Entity-Attributes/Conditions/List.md)   
4. ``LVL`` ``DURA``
5. Value   
6. ``LVL`` ``DURA``
7. Value   

````
FILE ---> COND BURNING LVL 3 AND DURA 5
FILE ---> COND BURNING DURA 3 AND LVL 5
````
  
---


  
### FLAG
1. ``FILE``
2. ``FLAG``
3. ``SWAP`` ``ADD`` ``REMOVE``
4. [Flag](../../CogsmosFramework/DemocrECS/Entity-Attributes/Flags/List.md)  

````
FILE ---> FLAG SWAP F_CHEAT_1_NO_CLIP
FILE ---> FLAG REMOVE F_8_IS_WALL
FILE ---> FLAG ADD F_8_IS_WALL
````
  
---
  


### PROP
1. ``FILE``
2. ``PROP``
3. ``SWAP`` ``ADD`` ``REMOVE``
4. [Property](../../CogsmosFramework/DemocrECS/Entity-Attributes/Properties/List.md) 

````
FILE ---> FLAG SWAP BURNABLE
FILE ---> FLAG REMOVE CONDUCTING
FILE ---> FLAG ADD BURNABLE
````
  
---
  


### UNIQ
1. ``FILE``
2. ``UNIQ``
3. [UniqueStatmod]()
4. (CONTEXTUAL) 

````
FILE ---> UNIQ DEAL_PLAIN_DAMAGE OF 20
FILE ---> UNIQ SPAWN_TILE_AROUND Terrain_0_0 3
FILE ---> UNIQ MOVE_SELECT END OF REACH

````
  
---
  


