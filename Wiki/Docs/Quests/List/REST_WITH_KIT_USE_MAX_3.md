

# Atlas Quests





### REST_WITH_KIT_USE_MAX_3
| Statname | Value | 
|  --  |  --  | 
| C_12_ATLAS_INDEX | REST_WITH_KIT_USE_MAX_3 | 
| C_72_LEC_META_USE | QUEST | 
| C_71_LEC_META_BY | RedRastaRigger(inhouse) | 
| C_6_NAME | Firestarter | 
| C_0_DESCRIPTION | Until Rest: Use at most 3x times a KitSet | 
| C_65_TIER | 1 | 
| C_14_LEC_RAW_DATA | [META{,   INDEX ---> REST_WITH_KIT_USE_MAX_3,   USE   ---> QUEST,   BY    ---> RedRastaRigger(inhouse), }, , , , //==============================================================================\\, //==============================================================================\\, //==============================================================================\\, , , , MAIN{, , , //------------------------------------------------------------------------------\\,   COMPONENTS[,     C_12_ATLAS_INDEX ---> REST_WITH_KIT_USE_MAX_3,     C_6_NAME ---> Firestarter,     C_0_DESCRIPTION ---> Until Rest: Use at most 3x times a KitSet,     C_65_TIER ---> 1, ,   ], , , //------------------------------------------------------------------------------\\,   FLAGS[,     F_18_QUEST,     F_19_UNIVERSAL_QUEST,   ], , , //------------------------------------------------------------------------------\\,   LISTENER[,     REST_WITH:,       MAX 3 ---> KIT_USE,     PERFORM:,       SELF ---> COMP C_9_CREDITS_ACCOUNT INCREMENT 100,       SELF ---> UNIQ DROP_LOOT_FILTER QUEST_KITPART_CORE,   ], }, , , , //==============================================================================\\, //==============================================================================\\, //==============================================================================\\, , , , REFERENCES{, , }, ] | 
| C_53_LISTENER | {PERFORM:[{operation:COMP, parameter:{compName:C_9_CREDITS_ACCOUNT, operand:INCREMENT, value:100}, typeOfCache:SELF}, {operation:UNIQ, parameter:{parameter:[QUEST_KITPART_CORE], type:DROP_LOOT_FILTER}, typeOfCache:SELF}], REST_WITH:[{comparator:3, flag:KIT_USE, operator:MAX}]} | 

