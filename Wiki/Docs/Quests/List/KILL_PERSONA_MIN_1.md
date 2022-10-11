

# Atlas Quests





### KILL_PERSONA_MIN_1
| Statname | Value | 
|  --  |  --  | 
| C_12_ATLAS_INDEX | KILL_PERSONA_MIN_1 | 
| C_72_LEC_META_USE | QUEST | 
| C_71_LEC_META_BY | RedRastaRigger(inhouse) | 
| C_6_NAME | Persona non grata | 
| C_0_DESCRIPTION | Kill 1: Wanted Persona | 
| C_65_TIER | 1 | 
| C_14_LEC_RAW_DATA | [META{,   INDEX ---> KILL_PERSONA_MIN_1,   USE   ---> QUEST,   BY    ---> RedRastaRigger(inhouse), }, , , , //==============================================================================\\, //==============================================================================\\, //==============================================================================\\, , , , MAIN{, , , //------------------------------------------------------------------------------\\,   COMPONENTS[,     C_12_ATLAS_INDEX ---> KILL_PERSONA_MIN_1,     C_6_NAME ---> Persona non grata,     C_0_DESCRIPTION ---> Kill 1: Wanted Persona,     C_65_TIER ---> 1, ,   ], , , //------------------------------------------------------------------------------\\,   FLAGS[,     F_18_QUEST,     F_20_SPECIFIC_1_MATRIX,     F_20_SPECIFIC_QUEST,   ], , , //------------------------------------------------------------------------------\\,   LISTENER[,     KILL:,       MIN 1 ---> FLAG HAS F_WANTED_PERSONA,     PERFORM:,       SELF ---> COMP C_9_CREDITS_ACCOUNT INCREMENT 100,       SELF ---> UNIQ DROP_LOOT_FILTER QUEST_KITPART_CORE,   ], }, , , , //==============================================================================\\, //==============================================================================\\, //==============================================================================\\, , , , REFERENCES{, , }, ] | 
| C_53_LISTENER | {KILL:[{comparator:1, flag:KILL, flags:F_WANTED_PERSONA, operation:FLAG, operator:MIN}], PERFORM:[{operation:COMP, parameter:{compName:C_9_CREDITS_ACCOUNT, operand:INCREMENT, value:100}, typeOfCache:SELF}, {operation:UNIQ, parameter:{parameter:[QUEST_KITPART_CORE], type:DROP_LOOT_FILTER}, typeOfCache:SELF}]} | 

