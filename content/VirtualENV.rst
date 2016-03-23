================================
Working with Virtual Environment
================================
:date: 2016-01-15 12:00
:category: Python
:author: Snehal Karale


In the Last article, I shared how I started my internship at Red Hat and my first day
at Red Hat.
Now its time to share what I learnt from the second day. I will not explain day by day,
rather particular topic that I was not heard about. So today I will explain Virtual
Environments in Python.

As the name virtual environment, you will get the idea its an isolated python environment.
So why we need isolated environment? When you are working on different python projects,
you can keep dependencies required by different projects in separate places. Virtual
environment solves the issue that one project needs one version of software or module
and another project requires a newer version of same. When a virtual environment is created,
it creates a directory which contains all executables that project would need.


------------------------------
How to use Virtual Environment
------------------------------
'virtualenv' is used to create virtual environment. Before using virtualenv, you need to
check whether virtualenv is installed or not.
Following command is used to install 'virtualenv'

$ sudo dnf install python-virtualenv

or you can use

$ pip install virtualenv


Once you done installation, start using it :)

I will eplain you step by step process to use virtualenv

1. Create your project directory and switch to it

                $ mkdir myproject

                $ cd myproject/

2. Once you switch to project directory, do following

                $ virtualenv myenv

                This will create directory named myenv in your myproject. You can check this by 'ls'

3. To activate Virtual Environment

                $ source myenv/bin/activate

                when you execute this, you will see following on your terminal

                        (myenv)[username@localhost myproject]$       

                Now you can start working on your project, you can install required packages that are
                specific to this project.

4. To deactivate Virtual Environment

                $deactivate

                Deactivating virtual environment brings you back in system's default python interpreter.

5. To delete Virtual Environment

                $ rm -rf myenv

                Delete directory created by virtualenv


This is how you can keep two different projectes isolated. 
