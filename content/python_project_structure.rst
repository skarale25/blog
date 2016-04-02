========================================
Creating Initial Python Project Structre
========================================
:Date: 2016-04-01 11:45
:Category: Python
:Author: Snehal Karale


In this blog I will share you how to create python project. When you start developing project in any language, there is some specific structure you have to define. 
The basic project structure looks as follows:


.. image:: /theme/images/icons/tree.png 
.. 

Follow the following steps to achieve above project structure.

1. Create your project directory and change the directory

    ``$  mkdir project``

    ``$  cd project/``

2. Create following directories under above project directory

    ``$  mkdir  docs  PROJ_NAME  tests``

    Here “PROJ_NAME”  should be your project name.
    “tests” directory will contain all unit test and other test for your project 

3. Create the python file under tests and PROJ_NAME

    ``$  touch PROJ_NAME/__init__.py``

    ``$  touch tests/__init__.py``

    In python __init__.py file is created to make directory as package.
    This file can be a empty file or can contain some initialization code.

4. Create setup.py file

    ``$  touch setup.py``    

    Setup.py file is created at root of project directory. This file is used to
    install python package. This file contains the setup() from setuptools and
    describes the metadata of project such as version, packages, name. This file
    is also used when you want to create python package.

5. Create README.rst

    ``$  touch README.rst``

    Python project should have README.rst file which describes the goal and basic
    information of project such as how to install project and how to run it. This
    file is not mandatory but this is important file, people will not take look on
    your project if your project don't have README.rst even if your project have
    great idea.   

6. Create MANIFEST.in

    ``$  touch MANIFEST.in``

    This file defines the list of file to be include in the package build.

This is the basic project structure which you can initiate and start your project.

