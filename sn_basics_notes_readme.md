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
* [ServiceNow Basics Module Recap](#service-now-basics-module-recap)
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


## ServiceNow Basics Module Recap

Core Concepts:

Personal Developer Instances are available free of charge from the ServiceNow Developer site

Instances hibernate when idle
Instances are reclaimed after ten days of inactivity
The ServiceNow user interface is made up of:

Banner
Application Navigator
Content Frame
The syntax open Incident > Open means to go to the Application Navigator, locate the Incident application, and open the Open module

Lists display records from a table, which are:

Searchable
Sortable
Editable (if permissions allow)
Filters display a subset of a table's records

Forms are used to create and edit records




## Contact
Created by [@Yahshemi](https://github.com/Yahshemi) - feel free to follow me!
