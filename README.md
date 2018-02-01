# Example-python-project-structure

This is a simple example of the overall organization of a Python project based on best practices.

* **./bin** - directory for storing binary files and for keeping executable files, primarily.
	* don't give executables .py extension, even if they are Python source files.
	* don't put any code in them except an import of and call to a main function defined somewhere else in projects
	* other folders containing non-essential programs can be /usr/bin, /usr/local/bin etc
* **./doc** - package reference documentation
* **./etc** - non-Python files that are to be regarded as external to the project source files, but have to be initialized with some values when application starts running
* **./lib** - static-link libraries, used for building .dlls, C extensions
	* stored files which containing machine code that cannot be executed directly
* **./project** - the code of interest
	* application startup registered in one of the scripts
	* don't put source in a directory called src or lib, this makes it hard to run without installing
	* if project is expressable as a single Python source file, then put it into the directory and name it something related to your project: Project/project.py
* **./project/test** - package integration and unit tests
	* test directory in one of two places: under the package directory containing test code and resources or as a stand-alone top level directory 
* **./project/native** - put non-Python sources such as C++ for pyd/so binary extension modules
* **./data** - may contain external data from third party sources, intermediate data, final processed data, original data and etc.
* **./scripts** - for that kind of command-line interface stuff
* **./var** - files that may be created or modified by the application during execution
* **.LICENSE** - lawyering up
* **.Makefile** - generic management tasks
* **.requirements.txt** - development dependencies
* **.setup.py** - package and distribution management

```
Project/
|-- bin/
|   |-- project
|
|-- doc/
|-- etc/
|-- lib/
|-- project/
|	|-- native/
|   |-- test/
|   |   |-- __init__.py
|   |   |-- test_main.py
|   |   
|   |-- __init__.py
|   |-- main.py
|
|-- data/
|-- scripts/
|-- var/
|-- .gitignore
|-- LICENSE
|-- Makefile
|-- README.me
|-- TODO.me
|-- requirments.txt
|-- setup.py

```