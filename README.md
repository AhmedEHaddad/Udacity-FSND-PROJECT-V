# Udacity-FSND-PROJECT-V
# Linux Server Configuration Project

Udacity: Full Stack Web Development Nanodegree

## Project Overview

You will take a baseline installation of a Linux server and prepare it to host your web applications. You will secure your server from a number of attack vectors, install and configure a database server, and deploy one of your existing web applications onto it.

## What you'll need (Pre-requisites):

1. Install [Vagrant](https://www.vagrantup.com/)
2. Install [VirtualBox](https://www.virtualbox.org/)
3. Go to [Udacity's Github](https://github.com/udacity/fullstack-nanodegree-vm) and clone or download it (contains all dependencies and libraries needed).
4. Add content of this [repository](https://github.com/AhmedEHaddad/Udacity-FSND-PROJECT-IV/tree/master/vagrant/catalog/catalogApp)

## How to run:

* simply visit the web app [URL](http://electroportal.eastasia.cloudapp.azure.com)
* clone this [repo](https://github.com/AhmedEHaddad/Udacity-FSND-PROJECT-IV/tree/master/vagrant/catalog/catalogApp) inside the `/vagrant/catalog` from this [Udacity's Repo](https://github.com/udacity/fullstack-nanodegree-vm)

* Launch the Virtual Machine using the command:
```
    $ vagrant up
```
* Run the application inside the Virtual Machine:
```
    $ python /vagrant/catalog/catalogApp/app.py
```
* Access application by opening [http://localhost:5000](http://localhost:5000).

## post-Deployment(Server) information:
* Public IP address: [52.184.24.170](http://52.184.24.170)
* URL : [electroportal.eastasia.cloudapp.azure.com](http://electroportal.eastasia.cloudapp.azure.com)

## Summary of software installed
* installed finger
* installed apache `apache2`
* mod_wsgi: `libapache2-mod-wsgi`
* POSTGRESQL
* GIT

## Summary of configurations made
* Start a new Ubuntu Linux server instance on [Microsoft Azure](https://portal.azure.com)
* updated all system packages right after installation as well as running auto remove.
* disabled remote login as `root`
* created the user `grader` in the `sudoers`
* disabled passwordauthentication and enforeced SSH-key Authentication.
* configured and and enabled the Uncomplicated Firewall (UFW) to only allow incoming connections on ports 2222, 80 and 123 while allowing all outgoing by default.
* changed SSH port from 22 to 2222
* web server responds to requests on port 80
* configure local TimeZone to UTC
* installed and configured database server
* installed and configured the item-catalog project to run as WSGI app web server.
* Make sure that your `.git` directory is not publicly accessible via a browser

## License
MIT
## Resources
* [Flask deployment](http://flask.pocoo.org/docs/1.0/deploying/mod_wsgi/)
* Udacity
