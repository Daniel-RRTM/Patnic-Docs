
# Race 
```
META
  INDEX         -->  ELF
  USE           -->  ACTOR_RACE
  BY            -->  RedRastaRigger(inhouse)
  DESCRIPTION   vvv

}

//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\

MAIN
//-------\\
  COMPONENTS
    C_12_ATLAS_INDEX     --->  ELF
    C_6_NAME             --->  Elf
    C_0_DESCRIPTION      --->  just like humans,but in tiny
    C_27_RACIAL_ENEMIES  --->  ELF
    C_28_RACIAL_FRIENDS  --->  ORC AND DWARF
    C_19_ATTRIBUTES      vvvv
      CON  --->  5
      AGI  --->  5
      REA  --->  5
      STR  --->  5
      WIL  --->  5
      LOG  --->  5
      INT  --->  5
      CHA ---> 5
//-------\\
  FLAGS
    F_6_ACTOR_ATTRIBUTES
    F_11_ACTOR_ATTRIBUTES_RACE

//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\

REFERENCE
END
```




# Role 
```
META
  INDEX         -->  ARSENIST_1
  USE           -->  ACTOR_ROLE
  BY            -->  RedRastaRigger(inhouse)
  DESCRIPTION   vvv

}

//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\

MAIN
//-------\\
  COMPONENTS
    C_12_ATLAS_INDEX     --->  ARSENIST_1
    C_6_NAME             --->  Arsenist T1
    C_65_TIER            --->  1
    C_0_DESCRIPTION      --->  Young teenager with behavioural problems and attention deficit
    C_47_SYNONYM         --->  Troublemaker AND Arsenist AND Firestarter
    C_37_M_TYPE          --->  MEAT
    C_19_ATTRIBUTES      vvvv
      CON  --->  5
      AGI  --->  5
      REA  --->  5
      STR  --->  5
      WIL  --->  5
      LOG  --->  5
      INT  --->  5
      CHA  --->  5
    C_20_SKILLBLOCK      vvvv
      SURVIVAL      --->  5
      SNEAKING      --->  5
      PERCEPTION    --->  5
      INTIMIDATION  --->  5
      COMPUTER      --->  5
//-------\\
  FLAGS
    F_6_ACTOR_ATTRIBUTES
    F_10_ACTOR_ATTRIBUTES_ROLES

//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\

REFERENCE
END
```



# Specialty 
```
META
  INDEX         -->  FECAL_ANALYCER
  USE           -->  ACTOR_SPECIALTY
  BY            -->  RedRastaRigger(inhouse)
  DESCRIPTION   vvv

}

//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\

MAIN
//-------\\
  COMPONENTS
    C_12_ATLAS_INDEX    --->  FECAL_ANALYCER
    C_6_NAME             --->  Fecal analycer
    C_14_SPECIALTY_NAME  --->  Fecal analycer
    C_50_ACTOR_ROLE_DESCRIPTION      --->  probably still earns as  mucg as your typicall wageslave
    C_47_SYNONYM         --->  bottle collector AND coupon collector AND dumpster diver
    C_37_M_TYPE          --->  MEAT
    C_19_ATTRIBUTES      vvvv
      CON  --->  5
      AGI  --->  5
      REA  --->  5
      STR  --->  5
      WIL  --->  5
      LOG  --->  5
      INT  --->  5
      CHA ---> 5
    C_20_SKILLBLOCK      vvvv
      SURVIVAL      --->  5
      SNEAKING      --->  5
      PERCEPTION    --->  5
      INTIMIDATION  --->  5
      COMPUTER      --->  5
//-------\\
  FLAGS
    F_6_ACTOR_ATTRIBUTES
    F_7_ACTOR_ATTRIBUTES_SPECIALTY

//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\
//----------------------------------------------------------------------------\\

REFERENCE
END
```