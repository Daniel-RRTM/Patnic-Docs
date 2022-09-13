

# **medical aid kit**


#### **Generall**
| Stat | Value | 
|  --  |  --  | 
| mechanical summary | recovers 5 Hitpoint of self, no move 1 round | 
| cooldown time | 4 | 
| decription | Standard-issue, containing bandages and most necessary drugs | 
| mod time | 1 | 
| rarity | 3 | 



#### **Event**
|  | **Seize** |  | 
|  --  |  --  |  --  | 
| Source |  | SELF | 
| Medium |  | SELF | 
| Reach |  | 1 | 
|  | **Consider** |  | 
| THIS | COMP | C_57_HITPOINTS NOT C_16_MAX_HITPOINTS | 
|  | **Perform** |  | 
| FILE | COMP | C_57_HITPOINTS INCREMENT 5 | 
| FILE | COND | INCAPACITATED 2 3 | 

-----

