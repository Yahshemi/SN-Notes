# Create the Need It Application

> ServiceNow's powerful platform allows developers to create cloud-native applications to rapidly add value to their organization. Developers can quickly create powerful applications using our Studio Integrated Development Environment (IDE) and a rich set of pre‑built services and templates. Also, because all applications are on our Platform, integrating with other ServiceNow applications is a breeze.


## Table of Contents
* [Designing an Application](#designing-an-application)
* [Application Scope](#application-scope)
* [Creating an Application](#creating-an-application)
* [Exercise: Create the Delete Me Application](#exercise-create-the-delete-me-application)
* [Contact](#contact)



## Designing an Application

Take time to design the application before building the application. Although the application strategy or requirements might change during development, it is more efficient to start with a well-defined plan.

At a minimum, plan the following:

- Business Logic
- User Interface (UI)
- Data Model

###### Business Logic
Be able to clearly state the business problem to be solved and the desired outcomes. For example, the business problem statement(s) may start with:

We need to track...
We need to automate...
We need to respond...
Your outcome statement(s) may start with:

We can save...
We can retire...
We can improve...
Be able to list all stakeholders for your application. Use this information to design user personas which are important when applying security to an application.

Clearly define the business process that will be part of the application. List the required steps, stakeholders, data sources, and outputs/visualizations.

###### User Interface
Decide what User Interfaces (UIs) you will use within your application. There are a variety of strategies in ServiceNow. Users' skill sets and requirements are part of the UI selection.

Decide if the application is for desktop and tablet only, or if users can access the application from a smartphone.

###### Data Model
Determine the data model for the application. Define the table structure the application will use as well as the relationships between the tables. Typically tables are the first artifact added to an application. Changing the data model during the application development process can cause extensive re-working of an application's logic.


## Business Problem
Service Requests for Human Resources, Facilities, Legal, and other departments have been managed by email, spreadsheets, and personal contact making them hard to track and report on. Requests have even gone unfilled and employees are dissatisfied with the process and outcomes. Mismanaging service requests has been very expensive for the company.

The NeedIt application will manage and track requests for Human Resources, Legal, Facilities, and one other department (to be determined) in an automated way, using an easy to use user interface that is consistent with other corporate software.

## Desired Outcomes
- A single location where employees can submit service requests for Human Resources, Legal, Facilities, and other departments.
- Accurate and timely completion of all tasks necessary to fulfill service requests; fewer missed deadlines.
- Retire the spreadsheets currently used to manage requests.
- Improve requestor satisfaction with process and request fulfillment.
- Automation of as many steps as possible.


## Application Scope

Applications created in Studio are known as scoped applications. Scope uniquely identifies every application file, not just within a single ServiceNow instance, but in every instance around the world. Why is this important?

- Scope protects an application, its files, and its data from conflicts with other applications.
- Scope determines which parts of an application are available for use by other applications in ServiceNow.
- Scope allows developers to configure which parts of their application can be acted on by other applications.
- Scope prevents work done in the main ServiceNow browser window (not in Studio) from becoming part of an application's files.

###### How is Scope Set?

Scope value is set automatically by ServiceNow when an application is created in Studio. Scope is constructed by concatenating 3 values:

- x_
- <value from the glide.appcreator.company.code system property>_
- <first_10_characters_of_app_name>
All scope values start with x_.

The glide.appcreator.company.code system property is a unique, two to five character value which ServiceNow sets to identify a company's instances as belonging to the same company. Your Personal Developer Instance (PDI) has a numerical glide.appcreator.company.code value, for example 27266.

The entire scope value cannot be longer than 18 characters.

If you create an application called Custom Robots on your PDI, the scope would be similar to:

x_27266_custom_rob

###### How Do I Know What Scope I am Working In?

When developing an application in Studio, the scope is automatically set to the application under development.

When working in a non-Studio ServiceNow window, be aware of which scope is active. ServiceNow warns you if you attempt to work on artifacts outside of the current scope.

In the example, a developer is attempting to modify the Incident list. The Incident application is a baseline ServiceNow application, which is part of the Global scope. The current scope is for the Custom Robots application, which means that an application file from the Incident application is out of scope. To resolve the problem, select a link in the warning message. Which link to select is determined by the use case.

To easily see which scope is the current scope without having to wait for a warning message, add the Application Picker to the ServiceNow Banner.

- In the main ServiceNow browser window, click the Settings icon (The settings icon is the rightmost icon in the ServiceNow banner.) in the ServiceNow Banner.
- Select the Developer pane.
- Enable the Show application picker in header option:
- Close Settings
- The Application Picker displays the name of the current application. If needed, use the Application Picker to change scope.


## Creating an Application

Use Studio to create applications. The process for creating an application is:

- Launch Studio.
- Click the Create Application button.
- Name and describe the application.
- Open the newly created application for editing in Studio or proceed through the Guided App Creator wizard.
The following example demonstrates the process for creating an application and opening it in Studio for editing. For details about Guided App Creator, refer to the Guided App Creator and ServiceNow Studio module within the Build My First Application course.

To launch Studio, use the Application Navigator to open System Applications > Studio.

Studio opens in a new browser tab and the Select Application dialog opens.

Click the Create Application button. Guided App Creator opens in a dialog. The Guided App Creator Welcome screen is shown if it is your first time opening Guided App Creator. Click the Let's get started button. If it is not your first time, you will see the General Info pane.

 NOTE: If you are using Microsoft Edge or Internet Explorer, you may only be able to work in the legacy application creator. If you are using Safari, you need version 12 or later to use Guided App Creator. To work in Guided App Creator, use a different browser.

- Name: application name
- Description: description of the application
- Drag and drop or browse to upload logo: image for the application
- Scoped/Global: scope for the application
- Scope: unique identifier for the application

Click the Create button.

Click the Continue in Studio (Advanced) link to open the Select Application dialog.

Click the Hello World link to open the new application.

The new application is loaded in Studio for development to begin. There are no default application files.

Configure the new application in the General Info pane.


## Exercise: Create the Delete Me Application


In this exercise, you will use Studio and Guided App Creator to create and delete the Delete Me application.


###### Create the Delete Me Application

- In the main ServiceNow browser window, use the Application Navigator to open System Applications > Studio.

- In the Select Application dialog, click the Create Application button.

- If you see the Guided App Creator Welcome screen, click the Let's get started button.

- Configure the application.

    Name:Delete Me
    Description: Temporary App

- Note the Scope value and its syntax. You do not need to do anything with this value, but it is important to understand for application file naming.

- Click the Create button.

- Click the Continue in Studio (Advanced) link to open the Select Application dialog.

- Click the Delete Me link to open the application in Studio for editing.

###### Delete the Delete Me Application
Delete the Delete Me application from the Application Settings record.

- In Studio, click the File menu and select the Settings menu item.

- Click the Delete button.

-In the Confirmation dialog, click the Delete button to confirm that you want to delete the application.

- When prompted, type the word delete into the dialog, then click the OK button.

- In the Progress dialog, click the Done button.

- Close the Studio browser tab.


## Contact
Created by [@Yahshemi](https://github.com/Yahshemi) - feel free to follow me!
