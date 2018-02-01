# example-python-project-structure

This is a simple example of the overall organization of a Python project based on best practices.

* ./project/ - the code of interest
* .LICENSE - lawyering up
* .setup.py - package and distribution management
* ./requirements.txt - development dependencies
* ./doc/ - package reference documentation
* ./project/test/ - package integration and unit tests
* .Makefile - generic management tasks
* .lib/ - static-link libraries, used for building .dlls, C extensions
* .data/ - data storage
* ./scripts or ./bin for that kind of command-line interface stuff
* etc

```
Project/
|-- doc/
|-- lib/
|-- data/
|-- scripts/
|
|-- bin/
|   |-- project
|
|-- project/
|   |-- test/
|   |   |-- __init__.py
|   |   |-- test_main.py
|   |   
|   |-- __init__.py
|   |-- main.py

|-- .gitignore
|-- LICENSE
|-- README.me
|-- TODO.me
|-- Makefile
|-- requirments.txt
|-- setup.py

```