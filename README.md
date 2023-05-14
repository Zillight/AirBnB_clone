https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/815046647d23428a14ca.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230514%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230514T151221Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=319784c6a93538a82cdd02646091ae213bfba767fa2eb3de26de40ab0ccb5ec2

Hbnb is a complete web application, integrating database storage, HTML/CSS templating, front-end and others.
This team project represents the first step towards building a full web application: the AirBnB clone.</br>
Although i did it myself just t have the repo in my github for saving purposes
This first step consists of:
- a custom command-line interface for data management,
- and the base classes for the storage of this data.

## Usage ���
The console works both in interactive mode and non-interactive mode, much like a Unix shell.
It prints a prompt **(hbnb)** and waits for the user for input.
Command | Example
------- | -------
Run the console | ```./console.py```
Quit the console | ```(hbnb) quit```
Display the help for a command | ```(hbnb) help <command>```
Create an object (prints its id)| ```(hbnb) create <class>```
Show an object | ```(hbnb) show <class> <id>``` or ```(hbnb) <class>.show(<id>)```
Destroy an object | ```(hbnb) destroy <class> <id>``` or ```(hbnb) <class>.destroy(<id>)```
Show all objects, or all instances of a class | ```(hbnb) all``` or ```(hbnb) all <class>```
Update an attribute of an object | ```(hbnb) update <class> <id> <attribute name> "<attribute value>"``` or ```(hbnb) <class>.update(<id>, <attribute name>, "<attribute value>")```
### Interactive mode (example)
```bash
$ ./console.py
(hbnb) help
Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
(hbnb)
(hbnb) quit
$
```
### Non-interactive mode (example)
```bash
$ echo "help" | ./console.py
(hbnb)
Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)
Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb)
$
```
## Testing :straight_ruler:
Unittests for the HolbertonBnB project are defined in the [tests]
To run the entire test suite simultaneously, execute the following command:
```
$ python3 unittest -m discover tests
```
Alternatively, you can specify a single test file to run at a time:
```
$ python3 unittest -m tests/test_console.py
```
