# Component  

## JSON
````  
"COMPONENT": {
    "prefix"      : ["SN: Component"],
    "description" : "Declare a new child of Component to describe a attribute of a Game-element\n",


    "body": [
        "extends Component",
        "class_name C_${TM_FILENAME_BASE/[C]//g}_${1/(.*)/${1:/upcase}/g}",								// {use_file_name ; select_C ; insert_blank}   {input_field_1 : called_name} 
        "",
        "var value: ${2:static_typing_preffered}",														// {input_field_2 : called_static_typing_preffered}
        "",
        "func _init(valuePara:${2/(.*)/${1}/g}) -> void :",												// {use_input_field_2 ; select_all ; insert_all}
        "	self.name = \"C_${TM_FILENAME_BASE/[C]//g}_${1/(.*)/${1:/upcase}/g}\"",							// {use_file_name ; select_C ; insert_blank}   {use_input_field_1 ; select_all ; write_upper_case}
        "	value     = valuePara",
        "",                                        
        "",                                       
        " ",                                        
        "",
        "static func getType_quack() -> String : return \"${2/(.*)/${1:/upcase}/g}\"",					// {use_second_input ; select_all ; writer_upper_case} 
        "",
        "",
        "static func getAutoDoc() -> Dictionary : ",
        "	return{",
        "	\"suggestion\"  : \"${3:write_one_sentence_here}\",",											// {input_field_3 : called_write_one_sentence_here}
        "	\"description\" : \"${4:write_one_sentence_here}\",",											// {input_field_4 : called_write_one_sentence_here}
        "	\"validInputs\" : ${5:[],   # references of ENUM-class only!}",									// {input_field_5 : called_reference_Array_of_valid_inputs_if_available}
        "	\"validType\"   : getType_quack(),",
        "	\"nameToShow\"  : \"${0:write_max_two_words_here}\",",											// {input_field_5 : called_write_max_two_words_here}
        "}",
        "",
        ""
    ]
}

````  

## GDS
````  

extends Component
class_name ________

var value: ________

func _init(valuePara:________) -> void :
	self.name = "________"
	value     = valuePara


 

static func getType_quack() -> String : return "________"


static func getAutoDoc() -> Dictionary : 
	return{
	"suggestion"  : "________________________________",
	"description" : "________________________________",
	"validInputs" : [________],   # references of ENUM-class only!
	"validType"   : getType_quack(),
	"nameToShow"  : "________________________________",
}

````  