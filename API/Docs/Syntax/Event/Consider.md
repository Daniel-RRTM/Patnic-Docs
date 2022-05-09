# Consider

### COMP  
Performance will be triggered if the Entity has this Component and the Condition are true.  
1. first has to be ``THIS``, then ``AND`` or ``OR``
2. ``COMP``
3. [Component](../../CogsmosFramework/DemocrECS/Entity-Attributes/Components/List.md)  
4. ``EQUALLS`` ``NOT`` ``LESS THAN`` ``MORE THAN``
5. Value  
(OPTIONAL)
6. can be multiple values, separated by ``AND``
  
````
THIS ---> COMP C_1_IS_WALKABLE EQUALLS TRUE
AND ---> COMP C_1_IS_WALKABLE NOT TRUE
AND ---> COMP C_11_RACE_NAME EQUALLS Orc AND Troll

OR ---> COMP C_48_RARITY MORE THAN 2
OR ---> COMP C_48_RARITY LESS THAN 5
````
  
---
  


### COND
Performance will be triggered if the Entity Condition is true and the additional values when stated.  
1. first has to be ``THIS``, then ``AND`` or ``OR``
2. ``COND``
3. ``IS`` ``NOT``
4. [Condition](../../CogsmosFramework/DemocrECS/Entity-Attributes/Conditions/List.md)  

(OPTIONAL,ONLY ONE)
  
5. ``AND``
6. ``LVL`` ``DURA``
7. ``LESS THAN`` ``MORE THAN``
8. Value

````
THIS ---> COND IS BURNING
AND ---> COND NOT BURNING

OR ---> COND IS WET AND LVL MORE THAN 2
OR ---> COND IS WET AND LVL LESS THAN 2

THIS ---> COND IS WET AND DURA MORE THAN 2
AND ---> COND IS WET AND DURA LESS THAN 2
````
  
---
  


### FLAG
Performance will be triggered if the Entity Condition is true.  
1. first has to be ``THIS``, then ``AND`` or ``OR``
2. ``FLAG``
3. ``HAS`` ``NOT``
4. [Flag](../../CogsmosFramework/DemocrECS/Entity-Attributes/Flags/List.md)  

````
AND ---> FLAG HAS F_CHEAT_1_NO_CLIP
THIS ---> FLAG NOT F_8_IS_WALL
````
  
---
  


### PROP
Performance will be triggered if the Entity Condition is true.  
1. first has to be ``THIS``, then ``AND`` or ``OR``
2. ``PROPERTY``
3. ``HAS`` ``NOT``
4. [Property](../../CogsmosFramework/DemocrECS/Entity-Attributes/Properties/List.md) 

````
THIS ---> FLAG HAS BURNABLE
THIS ---> FLAG NOT CONDUCTING
````
  
---
  


### TYPE
Performance will be triggered if the Entity Condition is true.  
1. first has to be ``THIS``, then ``AND`` or ``OR``
2. ``TYPE``
3. ``IS`` ``NOT``
4. ``ACTOR`` ``INTERACT`` ``TILE``

````
THIS ---> TYPE IS ACTOR
THIS ---> TYPE NOT INTERACTABLE
THIS ---> TYPE NOT TILE

````
  
---
  


