
# 0x00. AirBnB clone - The console



![alt text](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/65f4a1dd9c51265f49d0.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230807%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230807T202102Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=6f47a66ef01d62c895d5d438aa92f00740f3817bd49eb9595d305a79eb28fb26)

## Background Context

****Welcome to the AirBnB clone project!****

Before starting, please read the **AirBnB** concept page.

**First step: Write a command interpreter to manage your AirBnB objects.**

This is the first step towards building your first full web application: the **AirBnB clone**. This first step is very important because you will use what you build during this project with all other following projects: HTML/CSS templating, database storage, API, front-end integration…

Each task is linked and will help you to:

- put in place a parent class (called `BaseModel`) to take care of the initialization, serialization and deserialization of your future instances
- create a simple flow of serialization/deserialization: Instance <-> Dictionary <-> JSON string <-> file
- create all classes used for AirBnB (`User`, `State`, `City`, `Place`…) that inherit from `BaseModel`
- create the first abstracted storage engine of the project: File storage.
- create all unittests to validate all our classes and storage engine

****What’s a command interpreter?****

Do you remember the Shell? It’s exactly the same but limited to a specific use-case. In our case, we want to be able to manage the objects of our project:

- Create a new object (ex: a new User or a new Place)
- Retrieve an object from a file, a database etc…
- Do operations on objects (count, compute stats, etc…)
- Update attributes of an object
- Destroy an object
## How to install it

First, you need to clone this repository from Github

```
git clone https://github.com/ryackerman/AirBnB_clone.git
```
## How to use it

### Interactive mode

Your shell should work like this in interactive mode:

```
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
### Non-interactive mode

But also in non-interactive mode: (like the Shell project in C)

```
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

All tests should also pass in non-interactive mode: `$ echo "python3 -m unittest discover tests" | bash`

![alt text](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/815046647d23428a14ca.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230807%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230807T202102Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=8875e2bdd405b1bfa364b8643fe6820b160bc350f0ac146ed99af94d5aa68a9a)
## Commands

| **Commands**        | **Description**           |
| ------------- |:-------------:|
|quit or EOF|Exits the program|
|help	|Provides a text describing how to use a command. `help <command>`|
|create	|Creates a new instance of a valid `Class`, saves it (to the JSON file) and prints the `id`. Valid classes are: BaseModel, User, State, City, Amenity, Place, Review. `create <class name>`|
|show| Prints the string representation of an instance based on the class name and `id`. show <class name\> <id\> OR <class name\>.show(<id\>)|
|destroy| Deletes an instance based on the class name and `id` (saves the change into a JSON file). destroy <class name\> <id\>|
|all| Prints all string representation of all instances based or not on the class name. all <class name\>|
|update| Updates an instance based on the class name and `id` by adding or updating attribute (saves the changes into a JSON file). update <class name\> <id\> <attribute name\> "<attribute value\>"|
|count| Retrieve the number of instances of a class. <class name\>.count()|

## Tasks

    0. README, AUTHORS
    1. Be pycodestyle compliant!
    2. Unittests
    3. BaseModel
    4. Create BaseModel from dictionary
    5. Store first object
    6. Console 0.0.1
    7. Console 0.1
    8. First User
    9. More classes!
    10. Console 1.0
## Authors

- [ryackerman](https://github.com/ryackerman)
- [Mohamedkor2003](https://github.com/Mohamedkor2003)
