# AirBnB clone - The console

## Authors
---
* [Jorge Salazar](https://twitter.com/Jormao8)
* [Sara Hincapié](https://twitter.com/SaraHincapiMon1)
## Description
---
The AirBnB clone is for us to put in practice what we've learned so far, inheritance, classes, opening and closing files and changing them.
---
| File Name | Description and contents |
| --- | --- |
| [console.py](console.py) | This is the command interpreter file. |
| [amenity.py](models/amenity.py) | This file contains de class amenity. |
| [base_model.py](models/base_model.py) | This file contains de class base_model and its methods like save(), str(), dict(). |
| [city.py](models/city.py) | This file contains de class city. |
| [place.py](models/place.py) | This file contains de class place. |
| [review.py](models/review.py) | This file contains de class review. |
| [state.py](models/state.py) | This file contains de class state. |
| [user.py](models/user.py) | This file contains de class user. |
| [file_storage.py](models/engine/file_storage.py) | This file contains de class file_storage and its methods, like save(), reload(), all(). |
---
## The Console
The airbnb console (command interpreter) is to manipulate a powerful storage system, serializing and deserializing json files. The console can be run in two different modes, interactive mode and non-interactive mode.
## Installation
In order to run  the Airbnb console, you must "install" in your repository the console by cloning the following repository (shown below) in your machine running:
```
git clone https://github.com/jormao/AirBnB_clone.git
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
