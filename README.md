# How to Install Angular on Ubuntu

In this document, we will cover installation procedure of angular on Ubuntu 16.04 operating system

## Prerequisites

### System requirements

    * Ubuntu 16.04
    * 4 GB RAM
    * 10 GB free space

## Installation Procedure

To install angular cli we need nodejs and npm. First let’s understand what these are and why we need them.
What is Nodejs and Why you need for angular development?

Node.js is an open-source, cross-platform JavaScript run-time environment that executes JavaScript code outside of a browser. Node.js lets developers use JavaScript to develop wide variety of applications like network applications, command line tools, web api, web applications.

### What is npm and Why you need for angular development?

Npm stands for node package manager, it is a dependency management tool for javascript applications. This tool will help to install the libraries and other tools to support angular development.


## Install angular cli

* We will install angular cli using npm. On terminal run the install command shown below
You have to be in root to have the permission to run it.

```
$ sudo -s
$ npm install -g @angular/cli
```

* To test the @angular/cli 

```
ng version
```

## CREATING YOUR APPLICATION FOLDER

* Create angular application using ng new 
You should quit the root directory so you can create your project in your personal home directory

```
$ ctrl + d
ng new project_name
```

This command creates a new folder named project_name and creates all the files and setups the necessary libraries within this folder.

* Change to the project created by running these commands

```
cd project_name
ng serve -o
```

## CREATING AN ANGULAR COMPONENT IN UBUNTU

```
ng generate component component_name
```
From the code above, component_name is the name of your component.

## CREATING AN ANGULAR SERVICE IN UBUNTU

```
ng generate service service_name
```
From the code above, service_name is the name of your service.

## CREATING AN ANGULAR MODULE IN UBUNTU

```
ng generate module module_name
```
From the code above, module_name is the name of your module.


**EXPLANATION OF FOLDER CONTENTS:**

ng serve -o command starts webpack development server which in turn performs all the build process and opens a browser window and 
loads application url which runs at http://localhost:4200 by default.

* Search for the project you created and open it in VsCode.
  In the project opened, you have the below folders:

*e2e:* this folder contains end to end testing source and configuration code. If you wish to write end to end testing automation code, 
        your efforts go into this folder

*node_modules:* It contains all the project library dependencies. Files in this folder should not be modified as the changes 
                made are not guaranteed to be safe as updating/installing any other library can overwrite the changes made.

*src:* This is the folder that contains all your development effort. As an angular developer you spent lot of time 
       in this folder creating modules, components, services, directive etc.,


Within the src folder there are several other folders like

*app* – this folder contains all your source code, and this is the place all your development effort goes

*assets* – contains the static assets, like images etc.,

*environments* – contains the per environment configuration file which holds the settings to be used for dev/test and prod environments

## Other files are configuration files and settings.

**main.ts** is the starting file and the project code execution starts from this file.

Open *app.component.html*, delete the codes in it and add your own code


## UNINSTALLING ANGULAR IN UBUNTU

* Uninstall angular cli

```
 npm uninstall -g @angular/cli
```

## UNINSTALLING NODEJS IN UBUNTU

* Uninstall nodejs

```
sudo apt remove nodejs
```