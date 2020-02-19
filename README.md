# AirBnB clone - The console

## Authors
---
* [Jorge Salazar](https://twitter.com/Jormao8)
* [Sara Hincapié](https://twitter.com/SaraHincapiMon1)
## Description
---
The AirBnB clone is for us to put in practice what we've learned so far, inheritance, classes, opening and closing files and changing them.
---
## The Console
The airbnb console (command interpreter) is to manipulate a powerful storage system, serializing and deserializing json files. The console can be run in two different modes, interactive mode and non-interactive mode.
To use the console first clone the following repository.
```
git clone https://github.com/jormao/AirBnB_clone
```
### Interactive Mode
* To start the console in the interactive mode run.
```
./console.py
```
* use help to know the commands you can use in the console
```
help
```
#### Examples:
* show <class_name> <id>
```
(hbnb) show BaseModel 49faff9a-6318-451f-87b6-910505c55907
[BaseModel] (49faff9a-6318-451f-87b6-910505c55907) {'created_at': datetime.datetime(2017, 10, 2, 3, 10, 25, 903293), 'id': '49faff9a-6318-451f-87b6-910505c55907', 'updated_at': datetime.datetime(2017, 10, 2, 3, 10, 25, 903300)}
```
* create <class_name>
```
(hbnb) create BaseModel
49faff9a-6318-451f-87b6-910505c55907
```
* destroy <class_name> <id>
```
(hbnb) destroy BaseModel 49faff9a-6318-451f-87b6-910505c55907
```
* update <class_name> <id> <attribute_name> "<attribute_value>"
```
(hbnb) update BaseModel 49faff9a-6318-451f-87b6-910505c55907 name "Usuario"
```
### Non-interactive mode
* The non-interactive mode can be run two ways, having a text file with the command to run or using echo, then connecting them with a pipeline.
#### Examples:
* 
```
echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
```
*
```
cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
```