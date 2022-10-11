# PAIR
````
META
  INDEX --> C_S_1__M_1
  USE --> KITPART_MOD
  BY --> RedRastaRigger(inhouse)
  DESCRIPTION   vvv

}

//------------------------------------------------------------------------------\\
//------------------------------------------------------------------------------\\
//------------------------------------------------------------------------------\\

MAIN
//-------\\
  COMPONENTS
    C_6_NAME                     --->  enduring
    C_12_ATLAS_INDEX             --->  C_S_1__M_1
    C_0_DESCRIPTION              --->  Wheels of justice gind slow but grind fine
    C_35_KIT_MECHANICAL_SUMMARY  --->  your flame burns 10 Rounds but only does 1 damage
    C_48_RARITY                  --->  5
    C_37_M_TYPE                  --->  MAGIC
    C_31_KIT_CAT_TYPE            --->  SPELL
    C_38_KIT_PART_TYPE           --->  MOD
    C_36_KIT_MOD_TIME            --->  2
    C_33_COOLDOWN_TIMER          --->  4
    C_49_EVENT_REFERENCE         --->  C_S_1
  //-------\\
  FLAGS
    F_5_KITPART_TYPE
    F_16_KITPART_TYPE_MOD

//------------------------------------------------------------------------------\\
//------------------------------------------------------------------------------\\
//------------------------------------------------------------------------------\\

REFERENCE
END
````

# Event
````
META
  INDEX --> C_S_1__M_1
  USE --> EVENT
  BY --> RedRastaRigger(inhouse)
  DESCRIPTION   vvv

}

//----------------------------------------------------------------------------
//----------------------------------------------------------------------------
//----------------------------------------------------------------------------//

MAIN
//-------\\
  DATA
    MODIFICATION
      RUN ---> PERFORM -->   COND BURNING  LVL 1  AND  DURA 8
    ADDITION
      RUN ---> PERFORM -->   COND WET  LVL 1  AND  DURA 8
    DELETION
      RUN ---> PERFORM -->   COMP  C_57_HITPOINTS  DECREMENT BY 1

//------------------------------------------------------------------------------\\
//------------------------------------------------------------------------------\\
//------------------------------------------------------------------------------\\

REFERENCE
END
````