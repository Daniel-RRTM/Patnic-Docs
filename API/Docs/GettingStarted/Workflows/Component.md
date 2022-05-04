# Implementing Component 



1. Look up the Dictionary in ``/GameSrc/PatnicRoom/Indexes/EntityAttributes/Components.gd`` if there is allready a Component for your Idea. you can find an detailed description of each in  or XXX
2. If you there is no Component, you can create your own in ``/GameSrc/PatnicRoom/Components``
3. Name the file ``C_X`` with X for an unique number 
4. You can use the Template down below as starting point, or you can use our Snippet in our IDE
5. Make sure you declared all needed Data:
    * class-name like your file with an Name added in Caps (3 words at max)
    * Static typing of value when possible
    * self.name in _init() has class-name as value
    * dioJSONType_quack() return type in caps as String
    * all entries in getAutoDoc() are filled out
6. Add your Component in the Dictionary of ``/GameSrc/PatnicRoom/Indexes/EntityAttributes/Components.gd`` with its name as Key and class-reference as value
7. Test it by Instanciating, adding it to an Entity and getting it by a function  