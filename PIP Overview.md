Overview of pip

You have already learned that Python requires a driver to connect with a MySQL database. A driver is a library that allows you to interact with other software. Drivers come in the form of libraries, which are also called packages. 

Some drivers are not installed with your initial Python installation, so they need to be imported. These are called external libraries. To help manage these libraries, you should develop some familiarity with Pip, a built-in package installer that comes with your initial Python download. It can be used to install, configure and update external libraries.

 

Overview of Pip
Pip is a package management system that installs and manages Python packages in your system. A Python package refers to any external library that does not come with the initial Python download. 

Using pip to install your packages is a very easy way of ensuring that your environment has all the packages required to successfully run your application. 

To check which version of pip is installed in your environment, navigate to your command prompt and type pip –version. This command shows if you have pip installed and displays which version of pip is running on your machine. 

To access pip in the Jupyter environment, you can run the same command as before, but place a ! before pip as shown in the following code: 

1
!pip --version
Pip functionality
Pip has a host of useful commands which can simplify a programmer’s life by automatically configuring and installing them. Let's explore a few of these.


Installing a package

Installing a package using pip in the Jupyter environment is as simple as calling the pip install package using the following code:

1
!pip install mysql-connector

Viewing a package's information

You can then use pip to inform yourself of the particulars of a given package by using the SHOW command as follows:

1
!pip show mysql-connector
This command shows the following information:

Pip info
This information can help to confirm if you have the correct version of a library installed. A dependency is when one library is required by another library to run.

 

Updating libraries

Knowing the version numbers of a library can help with ensuring that your application runs smoothly. Libraries are constantly changing, and some changes can break your coding environment. 

If this occurs, then you may need to upgrade a given library. You can upgrade libraries using pip. To upgrade a library in pip you can type the following code:

1
!pip install --upgrade mysql-connector
This command ensures that the latest version of a library is present. 

 

Listing accessible packages in a working environment

Another useful function that comes with pip is that it can provide a list of all packages that are present in your working environment. To get a list printout of all libraries use the following code:

1
!pip list
This outputs a list of all packages accessible in this environment.

 

Listing accessible packages in the coding environment

To extract a list of libraries that are present in your coding environment to a text file use pip’s freeze method: 

1
!pip freeze >requirements.txt
This command first tells pip to extract all available packages. The angular bracket then directs pip to save the output in a text file called 'requirements.' You can determine where this file is stored by specifying a directory location for the file, as well as providing a custom name that is easily recognizable.

 

Removing a library from the working environment 

Finally, you can use the following code if you need to remove a library from your working environment:

1
!pip uninstall mysql-connector
With this command, pip finds the specified package and removes it from your system.

 

Conclusion
Pip is a versatile package manager that comes with Python. It can make a programmer’s life easier by providing useful methods for installing, configuring and updating third party libraries. 
