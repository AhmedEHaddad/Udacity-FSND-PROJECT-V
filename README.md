# Udacity-FSND-PROJECT-V
# Linux Server Configuration Project

Udacity: Full Stack Web Development Nanodegree

## Project Overview

You will take a baseline installation of a Linux server and prepare it to host your web applications. You will secure your server from a number of attack vectors, install and configure a database server, and deploy one of your existing web applications onto it.

## How to run:

* simply visit the web app [URL](http://electroportal.eastasia.cloudapp.azure.com)

## post-Deployment(Server) information:
* Public IP address: [52.184.24.170](http://52.184.24.170)
* URL : [electroportal.eastasia.cloudapp.azure.com](http://electroportal.eastasia.cloudapp.azure.com)

## Summary of software installed
* installed finger
* installed apache `apache2`
* mod_wsgi: `libapache2-mod-wsgi`
* POSTGRESQL
* GIT
* python3 & python3-pip
* python-pip
* the following dependencies using `pip` & `pip3`:
  ```
  pip3 install flask packaging oauth2client redis passlib flask-httpauth
  pip3 install sqlalchemy flask-sqlalchemy psycopg2-binary bleach requests
  ```


## Summary of configurations made
* Start a new Ubuntu Linux server instance on [Microsoft Azure](https://portal.azure.com)
* updated all system packages right after installation as well as running auto remove.
* disabled remote login as `root`
* created the user `grader` in the `sudoers`
* disabled passwordauthentication and enforeced SSH-key Authentication.
* configured and enabled the Uncomplicated Firewall (UFW) to only allow incoming connections on ports 2222, 80 and 123 while allowing all outgoing by default.
* changed SSH port from 22 to 2222
* web server responds to requests on port 80
* configure local TimeZone to UTC
* installed and configured database server
* installed and configured the item-catalog project to run as WSGI app web server.
* Make sure that `.git` directory is not publicly accessible via a browser

## License
* MIT
## Resources
* [Flask deployment](http://flask.pocoo.org/docs/1.0/deploying/mod_wsgi/)
* Udacity
* Stack server fault
