# ServiceNow Basics Objectives
> Getting Started with the basics.
In this module, you will learn to:

Identify the components of the ServiceNow user interface

Open modules using the Application Navigator

Use lists to open records for editing

Use filters to display a subset of a table's records

Open and use forms to create and edit records

> Live demo [_here_](https://developer.servicenow.com/dev.do#!/learn/learning-plans/rome/new_to_servicenow/app_store_learnv2_buildmyfirstapp_rome_personal_developer_instances).

## Table of Contents
* [Getting Around in ServiceNow](#getting-around-in-service-now)
* [Lists](#lists)
* [Filters](#filters)
* [Forms](#forms)
* [Setup](#setup)
* [Usage](#usage)
* [Project Status](#project-status)
* [Room for Improvement](#room-for-improvement)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)
<!-- * [License](#license) -->


## Getting Around in ServiceNow

There are three components of the ServiceNow user interface:

- Banner
- Application Navigator
- Content frame
###### Banner
The banner spans the top of every page. It contains a logo and global navigation controls. 
The controls are restricted based on user role. The admin user sees all of the controls. 
The Settings control (The Settings icon) contains a pane for setting developer options. 
The banner shows which user is logged in.

###### Application Navigator
Use the Application Navigator to access applications and modules (pages). 
Use the filter navigator field to quickly locate applications or modules. In the training modules, 
System Applications > Studio means to use the Application Navigator to locate the System Applications application, 
and open the Studio module by clicking on it.

###### Content Frame
The content frame displays content pages when users select modules in the Application Navigator. The pages in the content frame render data in many ways. The most basic page types are lists and forms.


## Lists
A list is a content page displaying zero or more records from the same table. Rows and columns organize the list. Each row is a record and each column is a field from the record. Lists are:

Searchable: Enter a value in the Search field
Sortable: Click the column label
Editable (if permissions allow): Double-click a field value


## Filters

Filters determine which table records are displayed in a list. When a developer creates a list module,
the filter conditions are set. In the example, only records with the Active field value of true appear in the list.
The syntax All > Active = true is known as a breadcrumb.

Users can create or modify filters. 

- Click the Filter icon (The Filter icon is a funnel) in a list.
- Set the [Field], [Comparison operator], and [Value] values.
- Use the AND button or the OR button to add additional conditions to the filter as required.
- Click the Run button to apply the filter to the list. 
Only records meeting the filter condition appear in the list and the breadcrumbs are updated.


## Forms

A form is a content page displaying fields and values for a single record from a database table. Forms have a 1-column layout, a 2-column layout, or a mix of both. Forms are opened from modules in the Application Navigator or by clicking a record's number in a list.
<!-- ![Example screenshot](./img/screenshot.png) -->
<!-- If you have screenshots you'd like to share, include them here. -->


## Setup
What are the project requirements/dependencies? Where are they listed? A requirements.txt or a Pipfile.lock file perhaps? Where is it located?

Proceed to describe how to install / setup one's local environment / get started with the project.


## Usage
How does one go about using it?
Provide various use cases and code examples here.

`write-your-code-here`


## Project Status
Project is: _in progress_ / _complete_ / _no longer being worked on_. If you are no longer working on it, provide reasons why.


## Room for Improvement
Include areas you believe need improvement / could be improved. Also add TODOs for future development.

Room for improvement:
- Improvement to be done 1
- Improvement to be done 2

To do:
- Feature to be added 1
- Feature to be added 2


## Acknowledgements
Give credit here.
- This project was inspired by...
- This project was based on [this tutorial](https://www.example.com).
- Many thanks to...


## Contact
Created by [@flynerdpl](https://www.flynerd.pl/) - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->