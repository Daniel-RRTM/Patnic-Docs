# **Your Wiki for everything in the Game!**
  
## **Hello there!**
We are happy you have found your way to the Game and eager to learn more about it!  
This Site is for **Players** and contains all **Game Elements** like Races, Tiles or Items.  
  
[**Click here**]() if you are looking for Docs of the technical Implementations.  
  
Both Sites are still under construction, we appreciate every feedback to improve its formatting, wording and Navigation! :)  

---
  
## **Getting Started**
P@tnicRoom breaks its Game Elements into very small pieces of attributes called **Components**. I.E. ``C_1_IS_WALKABLE = true``  
The number is not relevant for the Element, its used to make the Component itself unique and distinguishable.  
  
Components may get quickly underestimated because of their trivial scale, but they are more than the sum of their parts!  
By describing somethings attributes in such small steps, it gets compatible to interact with everything else in the Game, no matter its nature.
  
**The most often seen are:**  
  
[**Tiles**:](Overview_Enviroment.md) Grass, Concrete or Puddles  
[**Interactables**:](Overview_Enviroment.md) Automatons, Doors or Walls  
[**Actors**:](Overview_ActorAttributes.md) Humans, Ghosts or Computer-Viruses  
[**Kits**:](Overview_ActorAttributes.md) Gear, Talents, learned Skills  
  
---
  
## **Quickreferences**
  
1. **Entities** are set together by [**Templates**](), [**Components**](), [**Flags**]() and [**Properties**]().  
<br>  
  
2. **Chunks** consists of static [**Tiles**]() and wilingless [**Interactables**]().
    * They are saved in [**TileSets**](), named after its theme.  
<br>  
  
3. **Actors** get their values by [**Race**](), [**Role**]() and [**Specialty**]().
    * They can be procedurally generated with [**ActorSpawnTables**]().  
<br>  
  
4. **Kits** are used by Actors and the Player to survive and progress.
    * They need at least a [**Core**]() and optionally an [**Upgrade**]() and [**Trait**]().
    * Each plane of perceiption has three categorices:
        * [**Meat**]() has [**Meele**]() and [**Gun**]() and [**Armor**]()
        * [**Magic**]() has [**Infusion**]() and [**Spell**]() and [**Rite**]()
        * [**Matrix**]() has [**Cyberware**]() and [**Hack**]() and [**Drone**]()



