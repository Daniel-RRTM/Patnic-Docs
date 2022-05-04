# 006 - Condition

### Summary
This Module stores the different types of effects and contains the SubSystem to attach conditions to entities.  
  
  
### Functions
  
### attachConditionToEnt(Entity,condIndex,dura,lvl)
**1st Parameter :** Entity to affect  
**2nd Parameter :** [String of class of Conditions](../../CogsmosFramework/DemocrECS/Entity-Attributes/Conditions/List.md)  
**3rd Parameter :** int of rounds it affects Entity  
**4th Parameter :** int of intensity, has contextual significance or even not needed 
  
**Returns :**  void

Instanciates the Condition by the second parameter,  initialice the corresponding variables and connects it to broadcast-pattern 
  
````
for ent in API_004_KitSet.selection.triggers: 
		API_006_Condition.attachConditionToEnt(ent, para.condName, para.duration, para.level)
````
  
---  
  
