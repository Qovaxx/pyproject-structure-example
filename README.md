# Example-python-project-structure

This is a simple example of the overall organization of a Python project based on best practices.

* **./scripts** or **./bin** for that kind of command-line interface stuff
* **.data/** - data storage
* **./doc/** - package reference documentation
* **./project/** - the code of interest (don't put source in a directory called src or lib, this makes it hard to run without installing)
* **./project/test/** - package integration and unit tests
* **.lib/** - static-link libraries, used for building .dlls, C extensions
* **.LICENSE** - lawyering up
* **.Makefile** - generic management tasks
* **./requirements.txt** - development dependencies
* **.setup.py** - package and distribution management
* etc

```
**Project/**
|-- **bin/**
|   |-- project
|
|-- **data/**
|-- **doc/**
|-- **project/**
|   |-- **test/**
|   |   |-- __init__.py
|   |   |-- test_main.py
|   |   
|   |-- __init__.py
|   |-- main.py
|
|-- **lib/**
|-- **scripts/**
|-- .gitignore
|-- LICENSE
|-- Makefile
|-- README.me
|-- TODO.me
|-- requirments.txt
|-- setup.py

```