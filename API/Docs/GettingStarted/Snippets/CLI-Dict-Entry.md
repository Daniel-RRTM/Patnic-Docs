# CLI MetaData  

## JSON
````  
"CLI_SYNTAX": {
	"prefix"      : ["SN: 009 CLI dict entry"],
	"description" : "Add the neccessary Meta-data to the Command-dictionary to make it usable",


	"body": [
		"			\"${1:name_of_command}\" : {",
		"				 \"passive\"   : ${2:boolean   # describes if it needs to be turned off again}",
		"				,\"parameter\" : [${3:   # describes if it needs to be turned off again}]",
		"				,\"toString\"  : ${4:String   # will be shown in overview}",
		"				,\"class\"     : _API_017_Cmd_${5:ClassOfCommand   # Your class-name of the other snippet }",
		"				,\"list\"      : [${0:Array(s)   # insert here references vor suggested Parameter}] ",
		"				,\"input\"     : \"${1/(.*)/${1}/g}\"",
		"			},"
	]
}

````  

## GDS
````  

"name_of_command" : {
	"passive"     : ________
	,"parameter"  : [ ________, ________ ]
	,"toString"   : ________
	,"class"      : ________
	,"list"       : [ ________, ________ ]
	,"input"      : ________
},

````  
