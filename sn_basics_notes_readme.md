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
* [Adding a File to an Application](#adding-a-file-to-an-application)
* [Adding Fields to a Table](#adding-fields-to-a-table)
* [Adding Fields to a Table Recap](#adding-fields-to-a-table-recap)
* [Contact](#contact)

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


## Service Now Studio

Studio is ServiceNow's Integrated Development Environment (IDE). After creating applications in Guided App creator, use Studio to enhance and build on the applications. In Studio, lay out forms, create business logic, add or configure fields for tables, or create and edit application files.

To open Studio, use the Application Navigator to open System Applications > Studio. In the Applications list, click an application to open it for editing in Studio. The number of applications in your list may be different from the list shown.

Studio Anatomy
There are four components of the Studio user interface:

- Header
- Application Explorer
- Content Frame
- Status Bar


###### Header

The Header contains the name of the logged in user, menus, and controls.


###### Application Explorer

The Application Explorer contains a list of application files organized by category. Click an application file in the Application Explorer to open the file for viewing or editing in the content frame.

###### Content Frame

The content frame displays the form for each application file's record. The appearance and content of the form varies with file type. Each record appears in its own tab. A dot on a tab indicates unsaved changes.


###### Status Bar

The status bar contains information about the application name, application version, the number of files comprising the application, and the source control branch.



## Adding a File to an Application

To add an application file to an application in Studio, click the Create Application File link. The Create Application File dialog opens.

Use the Search field to locate the application file type, or browse the categories. Select the application file type, then click the Create button.

The new application file opens in a tab in Studio. The configuration options depend on application file type, such as table, module, or form.



## Adding Fields to a Table

As you have seen, fields can be added to tables when creating applications in Guided App Creator. After an application has been created, use Studio to modify table fields. There are several ways to add fields to a table. In the example, Form Designer is used to add table fields because it allows the form layout to be created at the same time fields are added.

Form Designer is a drag and drop interface used to:

Create form layouts
Create form views
Create and delete form sections
Add fields to tables
To open Form Designer in Studio, create a new form, or open an existing form for editing.

Click the Create Application File link.
Select Form and click the Next button.
Choose the form's table and click the Create button.
Form Designer opens in a new tab in Studio. Form Designer has three components:

- Header
- Field Navigator
- Form Layout

###### Header

The Header contains choice lists for selecting the table and view to configure. When changes have been made to a form, the header also contains the Undo and Save buttons.


###### Field Navigator

The Field Navigator contains two tabs:

Fields: List of all fields from the selected table that are not already part of the form layout.
Field Types: List of data types that can be used to create new table fields.


###### Form Layout

Forms are made up of fields and sections.


###### Add Fields
To add an existing table field to a form, click on the field in the Fields tab and drag the field to a location on the form. A blue highlight indicates a field can be dropped at that location.

To add a new field to a table, select the Field Types tab in the Field Navigator. Drag the data type for the new field to the form. A blue highlight indicates a field can be dropped at that location.

To configure a field hover over the field, then click the Edit field button (The Edit Properties button looks like a gear.) on the field.

Configure the properties for the new field. The properties vary depending on data type.

For all data types, provide a Label and a Name. The Label value is the human readable form of the field name. The Name value is used in scripts to reference the field. The Properties dialog will contain a suggested name like u_string_1. Replace that name with a name that makes sense. Do not use spaces or special characters except for the underscore (_).


DEVELOPER TIP: Capitalize only the first word of labels to be consistent with the ServiceNow baseline forms.

In the example, the maximum field length is 125 characters and the field is mandatory.

Close the Properties dialog by clicking the Close button (The close button is in the upper right of the Properties dialog.). The field is not saved to the table until the Save button is clicked in the header.

To remove a field from a form, hover over the form field until the Action buttons are enabled. Click the Delete button (The Delete button is on the right side of the field.). Removing a field from a form does not delete the field from the table.

Use the Form Designer to add, modify, or delete sections.

Use the View menu to create or edit a view.


## Adding Fields to a Table Recap

Core Concepts:

Use Guided App Creator to create applications.

- Add application roles
- Create tables

The data model design determines what tables and fields an application needs.

Studio is the Integrated Development Environment (IDE) for continuing development on applications.

Use Studio to create application files.

Use Form Designer to:

- Add fields to tables
- Create form layouts
- Create form sections
- Create form views


## Contact
Created by [@Yahshemi](https://github.com/Yahshemi) - feel free to follow me!
