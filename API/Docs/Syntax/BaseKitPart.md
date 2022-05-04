# Pair
````
META
  INDEX         -->  C_I_1
  USE           -->  KITPART_BASE
  BY            -->  RedRastaRigger(inhouse)
  DESCRIPTION   vvv

}

//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\

MAIN
//-------\\
  COMPONENTS
    C_6_NAME                     --->  4th Wallbreak
    C_12_ATLAS_INDEX             --->  C_I_1
    C_0_DESCRIPTION              --->  //TODO: add description
    C_35_KIT_MECHANICAL_SUMMARY  --->  deals 10 structure-pointts damage, 20 for thin walls
    C_48_RARITY                  --->  3
    C_31_KIT_CAT_TYPE            --->  INFUSION
    C_37_M_TYPE                  --->  MEAT
    C_38_KIT_PART_TYPE           --->  BASE
    C_36_KIT_MOD_TIME            --->  3
    C_33_COOLDOWN_TIMER          --->  1
    C_49_EVENT_REFERENCE         --->  C_I_1
//-------\\
  FLAGS
    F_5_KITPART_TYPE
    F_15_KITPART_TYPE_BASE

//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\

REFERENCE
END
````

# Event
````
META
  INDEX         -->  C_I_1
  USE           -->  EVENT
  BY            -->  RedRastaRigger(inhouse)
  DESCRIPTION   vvv

//----------------------------------------------------------------------------
//----------------------------------------------------------------------------
//----------------------------------------------------------------------------//

MAIN
//-------\\
  SELECT
    SEIZE
      MEDIUM  --->  LINEA
      SOURCE  --->  SELF
      REACH   --->  2
    CONSIDER
      THIS    --->  FLAG  -->  F_8_IS_WALL
    PERFORM
      CACHE   --->  SET   -->  THIS  ->  FILE  
//-------\\
  RUN
    PERFORM
      FILE  --->  UNIQ --> SPAWN_TILE OF Suburban_0_0

//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\

REFERENCE
END
````
























