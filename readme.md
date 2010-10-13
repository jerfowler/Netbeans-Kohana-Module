# Netbeans Module for the [Kohana PHP Framework](http://kohanaframework.org/).

Version 1.1, Built for Nebeans 6.9.1

This Module currently only has:

## Project

*	Sample Kohana 3 Project

## Templates

*	Controller
*	Controller (AJAX)
*	Model (ORM)
*	View (HTML5)
*	View (HTML4)
*	View (EMPTY)

# Installation

1. Download the .nbm file in the build directory.
2. Open the Plugin dialog in Netbeans under Tools | Plugins
3. Under the Downloaded tab, click the Add Plugins button
4. Open the downloaded .nbm file from step 1
5. Click the Install button
6. Follow along with the prompts to install

# Usage

## Projects

Create a new project in Netbeans, Select the PHP Category and choose Kohana 3 Project

Be sure to pull for latest updates
		git pull 
		
Then download the latest core and modules
		git submodule init 
		git submodule update 

## Templates

Create a new PHP Project or open an existing one. Browse to where you want the new file and click the New File button. 
Select one of the new templates under the Kohana 3.x Category.

*	Be sure to use all lowercase letters with new file names. The Template will then captitalize the name. 
*	If creating a controller within a subdirectory, best to name the file the entire directory structure first so the template populates correctly. Then Refactor the file to rename it.
	
Example: 

Directory is \controller\admin\page, name the file admin_page. 
This will then populate the controller template correctly. 
Then rename the file to just "admin".

### Template variables

Netbeans provides support for the FreeMarker Template Engine which supports variables. These variables can be set 
in the *User.properties* file in Template Manager. To open Template Manager, click Tools | Templates menu item. 

User.properties is located under *User Configuration Properties* in the Templates tree structure.

### Variables used in the templates:

These are specified in the Project's properties

		project.name
		project.encoding

A default user variable is provided to Netbeans by the operating system, but it should probably be modified in User.properties to include more details

		user=Jeremy Fowler <jeremy.f76@gmail.com>

These can be specified in User.properties

		project.description=Kohana PHP Project
		project.keywords=Kohana,PHP
		project.copyright=(c) Jeremy Fowler
		project.license=http://creativecommons.org/licenses/BSD/

Unique values can be assigned to projects by appending the project name on the end.

Example Kohana PHP Project named MyProject:

		project.description.MyProject=My Unique Project Description
		project.keywords.MyProject=MyProject,Kohana,PHP
		project.copyright.MyProject=(c) MyProject Team
		project.license.MyProject=http://myproject.org/license.php


# More to come...

*	More Model Templates: Sprig, Jelly, Hive
*	More Specialized Controller Templates: REST, AUTH, etc...
*	Other stuff as I learn it.... (suggestions anyone?)
