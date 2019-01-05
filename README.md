# Introduction
In the Linux Server Configuration project, we are asked to deploy a Linux web server using a web service provider e.g. Amazon Web Services (AWS). We are asked to configure the server details which will be mentioned below in this file.

# Linux Server information
Some of the following will be needed to acccess the web server:

* Server IP Address: 3.8.134.109 , SSH Port: 2200.
* Web Application URL: http://3.8.134.109.xip.io/

* Installed Software:
-Git version control system.

-Finger program which provides the command `finger` that is used to find information about computer users.

-Pip which is a package manager for python packages, provides the command `pip` which can be used to install python packages.

-PostgreSQL which is an open source database system, the PostgreSQL command line was installed to complete this project.

-Apache2 Web Server which is requires to deploy a server on Linux systems, Ubuntu was used in my case.

-Web Server Gateway Interface (WSGI) which is a calling convention that is used to make web servers like Apache host and interact with a python-written application.

* Configuration Changes:
-The SSH port was changed from the default (22) to a custom (2200).

-Password authentication had been disable and instead, key-based authentication is used to login to the server, the command `ssh <user>@<ipAddress> -p <portnumber> -i <key-combination-path>` is used to login using key-based authentication.

-A new user _grader_ has been created and it has been given the sudo access.

-The uncomplicated firewall (UFW) was configured to only allow incomming connection for SSH (port 2200), HTTP (port 80), NTP (port 123).

* Third-party resources used to complete this project:

1. Amazon Lightsail which is provided by Amazon Web Services [AWS](https://aws.amazon.com/lightsail/).
2. GitHub is used to clone my Item Catalog Project [repository](https://github.com/Saudrules/Item-Catalog).
3. [This](http://flask.pocoo.org/docs/1.0/deploying/mod_wsgi/) mod_wsgi (Apache) documentation was used to complete this project.
4. [Dillinger](https://dillinger.io/) editor was used to preview the README content before submission.
* SSH key created for the _grader_ user can be found in: `~/.ssh/authorized_keys`. 
