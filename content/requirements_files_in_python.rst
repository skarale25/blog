===========================
Requirement Files in Python
===========================
:date: 2016-01-22 12:00
:category: Python
:author: Snehal Karale



When you are setting up an application on new system, you have to install bunch
of dependencies i.e. bunch of packages required by that application. So it is
difficult to find the dependencies or to remember the dependencies every time
before installation. So Solution is here :) And Requirement files comes in the
picture here. Python provides the way to freezing the required packages in single
file and run that file on every new system to install  an application. Now you get
the idea, what this blog is about. So in this blog, I am going to talk about
requirement files in python. Let's start.......

Up till now you get the idea about what is requirement file, so we will go with some
technical details.Requirement files contain a list of packages to be install using pip
install.


-------------------------
Freezing the requirements
-------------------------
How to create requirement.txt? To create requirement.txt use following command,

$ pip freeze > requirement.txt

The above command will freeze i.e. collect the packages and copied and save in requirement.txt

when you run

$ pip freeze

in your current development environment, it will gives you list of packages with versions. For Example-

Markdown==2.6.5

pelican==3.6.0

The idea behind requirement file is, making repeatable installations.

Once your requirement file is ready, you can install it on other system using following-

$ pip install -r requirement.txt

Requirement files create a environment required to run your application. This is what I learnt and implement in second week.
