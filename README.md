<a href="https://github.com/dilip-987/admin-guide/blob/19c065ccae1a7a8ecdee3480bfdb7ecd8378395b/ignatius-logo-black.svg?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/19c065ccae1a7a8ecdee3480bfdb7ecd8378395b/ignatius-logo-black.svg?raw=true" width="300" alt="n8n.io - Screenshot"></a>

## 1.1 Purpose of this User Guide

This document is a user reference for the Ignatius system, providing explanations for all features of the application and the instructions to use these features.

The audience primarily includes client users that will be administering the system. This document is meant to be a guide for understanding how the system works and how an admin user can configure its many features.

For new Admin users, this User Guide outlines how to access and use the many features, and explains navigation and terminology. The guide will include the following and more:<br />
    • Creating and managing applications<br />
    • Creating and managing Tables<br />
    • Managing Fields, forms, reports and relationships between Tables<br />
    • Importing and exporting data into the Tables<br />
    • Creating Custom pages as home pages<br />
    • Managing users, user roles and user permissions<br />

<b>Note:</b> The <b>Ignatius API Documentation</b> Guide is available for instructions on how to use API Commands to add, modify, delete, or query tables, reports, charts, fields, forms, relations, and notifications within the database.

# Chapter 2 – Using the Admin App
##   2.1 Overview
The Ignatius Application is used to build database applications to support business requirements. The Applications are used to store, and manage data for business needs. 

Within the Ignitatius Application, multiple database applications can be set up to meet different business or operational requirements. Applications can represent any desired independent entity such as companies, organizations, projects etc... Applications can be viewed as databases that are maintained separately since they support different requirements and can simplify administration when managed as separate entities.

The Admin App is where all applications are created and managed along with the database tables, reports, users and other admin related functions within a specific application. All applications will be accessible via the Admin App. Each Application will have its own database structure with its specific tables, table fields, forms and reports. Each Application can also have its own authorized users. 

An Admin user has access to all applications, while non-admin users can be set up to only have access to specific applications.

Each Application will have the following features. Instructions for all features will be discussed in the subsequent chapters of this guide.<br />
    • <b>Tables</b> store your data into rows (records) and columns (fields). Each field contains a single piece of data and holds a particular type of data (i.e. Text, Numeric Data, Date, Currency etc..).<br />
    • <b>Relationships</b> are used to represent a connection between two tables. A table-to-table relationship is used to better organize your data, and reference data existing in another table rather than repeating the same data in multiple tables.<br />
    • <b>Forms</b> are used are data entry forms used to enter data into tables. Forms can be set up to display certain fields for data entry. <br />
    • <b>Data Import</b> is set up to pull data from files or URL locations into tables.<br />
    • <b>Reports</b> are used to view/display data from your tables. You can create different types of reports based on your needs.<br />
    • <b>Roles</b> represent a collection of user permissions. Roles dictate what actions users are allowed to perform or what users are able to see within an application.<br />
    • <b>Users</b> are people who have access to the applications. Users will be assigned a user role that will define their permissions within an application.<br />
    • <b>Notifications</b> are used to alert users when records have been updated on a table. <br />
    • <b>Pages</b> are custom pages usually set up as Home pages for the applications. These pages can be any custom HTML page or Dashboards to give an overview of your data.<br />
    • <b>Power BI Reports</b> are reports available through Power BI, the business analytics service that is integrated with Ignatius.<br />
 
## 2.2 Dashboard
The dashboard is the first screen that appears following user login. It displays various types of summary information.

<a href="https://github.com/dilip-987/admin-guide/blob/074894641ed97999700363084d0cc4d753669722/2.2.1.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/074894641ed97999700363084d0cc4d753669722/2.2.1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

## 2.3 Navigation

The application contains various features for navigation which include the menu, buttons, and breadcrumbs.

<a href="https://github.com/dilip-987/admin-guide/blob/074894641ed97999700363084d0cc4d753669722/2.2.2.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/074894641ed97999700363084d0cc4d753669722/2.2.2.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

### 2.3.1 Menu

The menu can be found along the left side of the screen. Clicking on a menu item will either produce a new set of items or expand a drop-down menu, as shown in the figures below.

The content in the main window will change to correspond with the menu item that you selected.

<a href="https://github.com/dilip-987/admin-guide/blob/074894641ed97999700363084d0cc4d753669722/2.2.3.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/074894641ed97999700363084d0cc4d753669722/2.2.3.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


### 2.3.2 Buttons

Buttons appears in various places throughout the app, such as the Add Field button on the Fields screen:

<a href="https://github.com/dilip-987/admin-guide/blob/074894641ed97999700363084d0cc4d753669722/2.3.1.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/074894641ed97999700363084d0cc4d753669722/2.3.1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



### 2.3.4 Breadcrumbs

The breadcrumb feature can be seen at the top of most pages, as shown in the figure below. With it, you can see where you are in the application hierarchy.
You can also click on any of the items in the path to navigate immediately to the desired page.

<a href="https://github.com/dilip-987/admin-guide/blob/074894641ed97999700363084d0cc4d753669722/2.3.2.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/074894641ed97999700363084d0cc4d753669722/2.3.2.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



# 2.4 Applications

Applications represent the different database applications created to meet your requirements. Applications can represent any desired independent entity such as companies, organizations, projects etc... Applications can be viewed as separate databases that are maintained separately since they support different requirements and can simplify administration when managed as separate entities.

Each Application created will have its own database structure with its own schema, tables and table fields. Applications created are independent of one another.

The Applications Page can be accessed via the Menu on the left side of the screen.
The Applications Page will display the different applications currently created in your environment.


<a href="https://github.com/dilip-987/admin-guide/blob/b264631a15503ee6a0d0da14608321cdca7ba9a5/4.2.application.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/b264631a15503ee6a0d0da14608321cdca7ba9a5/4.2.application.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

## 2.4.1 Accessing an Application

To access an application:
    1. On the Applications Page, locate the application you wish to access. Click View Application below the desired application.

The page displayed will show the tables created for that application (if any), along with many actions that can be taken to manage the database tables.

<a href="https://github.com/dilip-987/admin-guide/blob/b264631a15503ee6a0d0da14608321cdca7ba9a5/2.4.access-application.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/b264631a15503ee6a0d0da14608321cdca7ba9a5/2.4.access-application.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


## 2.4.2 Creating and Deleting an Application
<u><b>To create a new application:</b></u>
  1. On the Applications Page, click Add Application at the top right of the screen.

<a href="https://github.com/dilip-987/admin-guide/blob/c96fae5642a6fb9a3def12aaa1c90846e5f3130a/2.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/c96fae5642a6fb9a3def12aaa1c90846e5f3130a/1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

  2. On the pop-up window displayed, enter the Name of the Application you wish to add.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/2.4.2(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/2.4.2(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>  
  
   3. Click Save. The Application will then be visible and accessible from the Applications Page. Tables can then be added to the Application as needed.

<u><b>To delete an application:</b></u></br>
    1. On the <b>Applications Page</b>, click the X icon (Delete Icon) next to the desired application.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/2.4.2(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/2.4.2(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


   2. On the pop-up window displayed, click <b>Okay</b> to confirm.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/2.4.2(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/2.4.2(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

## 2.4.3 Navigation within an Application

Once within a desired application, a <b>Default Dashboard Page</b> will be displayed if one was created for that application, or the <b>Tables Page</b> will be displayed. The <b>Tables Page</b> displays the list of tables currently created for an application.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/2.4.3.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/2.4.3.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

On the left-side panel of the screen, a menu is displayed with links to the Application’s Tables, Custom Pages and Reports, as well as the Application’s Settings.


Clicking on a Table Menu Item will expand a drop-down menu with options to manage that table. 

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/2.4.3(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/2.4.3(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


# Chapter 3 – Managing Tables

In this chapter, you’ll learn how to do the following within a specific application:

    • Add a table

    • Add fields to a table

    • Add a relationship between tables

    • Create Lookup Fields and Summary Fields

    • Import data into a table

    • Establish a refresh schedule for a data import

    • Establish a Schedule for Data Purge

    • Delete table elements and an entire table

    • View a Table

    • Create and Manage Reports

    • Create and Manage Forms

## 3.1 Add a Table

An application may have one or more tables. You can add, delete, and configure the tables in any application you have access to.

To add a table to an application:
    1. On the Applications Page, locate the application to which you wish to add a table, and select the View Application link to access the application.

    2. Once in the desired application, select App Settings from the left sidebar menu. 

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/3.1.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/3.1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    3. On the App Settings Page, select the Tables Tab.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/3.1(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/3.1(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    4. On the Tables Tab displayed, click Add Table at the upper-right corner of the screen. This will display an Entry Form.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/3.1(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/3.1(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    5. On the Entry Form displayed, enter a name for the table that is descriptive (e.g. “Components”) and click Save Changes.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/3.1(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/3.1(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    6.     6. The Table added will now be displayed on the sidebar menu at the left of the screen, as well as on the Tables Tab on the App Settings Page. 
The table added can now be configured as needed with fields.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/3.1(4).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/3.1(4).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


## 3.2 Add Fields to a Table

A table consists of one or more fields. You can add, delete, and configure the fields in any table. 

To add fields to a table:
    1. On the left sidebar menu, click the drop-down arrow next the table to which you wish to add a field. This will display the list of actions that can be taken for the table.


<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.2.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.2.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    2. Click Manage Fields. This will display the selected Table’s Fields Page. This page will display the existing fields on the table if any.


<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.2(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.2(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. Click Add Field in the upper-right corner of the page. This will display an Entry Form.




<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.2(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.2.png(2)?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    4. On the Entry Form displayed, enter a descriptive Field name such as “Component Name”, then select a Field Type.



<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.2(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.2(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


   
    A Field Type specifies and constrains what kind of data is to be kept in a field. The following field types are available:

    • Text			: 	Data contains alphanumeric characters
    • Text Multi-Line		:	Data contains text on multiple lines
    • Text Multiple Choice	:	Data contains specific values (example A or B or C)
    • Numeric		:	Data only contains numeric values
    • Currency		:	Data is a currency
    • Datetime		:	Data contains a date and time
    • Date			:	Data contains a date without the time
    • Checkbox		:	Data is one of two values (example Yes or No)
    • File Attachment	:	Data is a file
    • User			:	Data is an existing user in the application

In addition, the following formula field types are also available, and can be used to apply operations to existing fields:

    • Formula – Text 		:	Applies formulas to Text Fields 
    • Formula – Numeric	:	Applies formulas to Numerical Fields
    • Formula – Currency	:	Applies formulas to Currency Fields
    • Formula – Date		:	Applies formulas to Date Fields

Note: For more details on Formula Fields, please refer to the Formula Fields Documentation.

5. Check the ‘Must Be Unique’ checkbox if the field requires a “unique constraint”. The unique constraint will ensure that all values entered on the table for that field are unique values (i.e. this prevents duplicate values). 
Note: Fields marked as unique can also be used as key fields/reference fields to set up relationships between tables. This will be discussed in the Section on Table Relationships.

6. Once the Field Name and Field Type are entered, click Save Changes. The added field will now be listed on the Fields Page for the selected table.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.2(4).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.2(4).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


7. Continue to add more fields as needed by repeating steps 3-6.


## 3.3 Add a relationship between tables

A relationship is a connection between two tables. A table-to-table relationship is used to better organize your data, and reference data existing in another table rather than repeating the same data in multiple tables.

By referencing data from another table, you will save time by avoiding entering the same information in another table.

Example: A customer table maintains the customer contact information, and address. A customer can place several orders that are stored in an Order table. Adding a relationship between the customer table and the order table will organize your data and save you time because you will not have to re-enter the same customer info for every record in the order table. With a relationship between the customer and order table, you will be able to simply link order records to the corresponding customer records.

To establish a relationship between two tables:
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Relations. This will display the Table Relations Page.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



   
    2. On the Table Relations Page, click Add Relation at the upper-right corner.


<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    3.On the Create Relations Page displayed, under Table Name:

Click the drop-down option to select the other table to which you wish to create a relationship.


<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    4. Once the table is selected, on the Create Relations Page, under the section named “for this relation, which is true?”:

Select the parent-child relationship you wish to create between the two tables by selecting one of the relationship options displayed on the screen.
For example: a customer can place many orders (hence a customer can have many order numbers), but order numbers are unique (hence one specific order number is only assigned to one specific customer). In this case, the relationship option would be as follow: Each Customer may have many Orders.


<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


n this case, since a customer can have many orders, the customer represents the parent table, and the order represents the child table.


<a href="https://github.com/dilip-987/admin-guide/blob/fc3bac04d72b92606de2a8d9f41c2f9c7de796cd/ss.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/fc3bac04d72b92606de2a8d9f41c2f9c7de796cd/ss.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    5. On the Create Relations Page, under Parent Table:

Select the Key Field of the parent table. The key field is the unique identifier (Unique ID) assigned to each distinct element in a table. For example, the unique Customer ID given to each customer represents the Key Field of the customer table.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(4).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(4).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



Next on the Create Relations Page, under Child Table, the Field specified represent the name of the reference field that will be added to the child table. This field will relate to the key field in the parent table.

In the example screenshot below, the field Related Customer will be added to the Order Table and will reference the Customer ID (Key Field of the Customer Table (Parent Table)).

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(5).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(5).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>




    6. OPTIONAL STEP: In addition to creating a relationship and adding a reference field, you will also be able to create Lookup Fields:

    • A Lookup Field is a read-only field that displays information pulled from a reference table (parent table). When a record is created in a child table, lookup fields will be automatically populated with the info pulled from the parent table. 

For example, customer info such as First Name, Last Name, Address will be automatically pulled from the customer table, and populated onto the order table based on the Reference Field Customer ID.

If you do not wish to create Lookup Fields, skip this step and continue to the next step below. 

Note: Lookup fields can be added at any point by editing the table-to-table relationship.

Note: Lookup fields can be added at any point by editing the table-to-table relationship.

To create a lookup field: 
    • On the Create Relations Page, under Child Table, Click the Add Lookup Field button.


<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(6).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(6).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    • Click on the drop-down option to select the Lookup Field you wish to add to the child table.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(7).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(7).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    • Continue to add other lookup fields if desired by using the + option. Add/Remove fields by using the +/– options.
    • Click Save when done. 

    7. Once the relationship details are added, Click Save on the Create Relations Page. The Relationship created will now be displayed on the Table’s Relations Page. 

Note: The relationship can be edited at any point from there by clicking the edit icon	 next to the relationship record on the Relations Page

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(8).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(8).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


Once the relationship is created, the reference fields and lookup fields (if any) will be automatically added to the child table (the table referencing the information from the parent table).
In the example screenshot below, the field Related Customer was automatically added to the Order Table to reference the Key Field (Customer ID) of the Customer Table.


<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(9).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.3(9).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


## 3.4 Create Lookup Fields

As mentioned in the table-to-table relationship section, a Lookup Field is a read-only field that displays information pulled from a reference table (parent table). When a record is created in a child table, lookup fields will be automatically populated with the info pulled from the parent table. 

For example, customer info such as First Name, Last Name, Address will be automatically pulled from the customer table, and populated onto the order table based on the Reference Field Customer ID.

Lookup Fields can be added when creating a relationship between two tables or by editing an existing table-to-table relationship. Please refer to the section “Add a Relationship between Tables” if you need to create a table-to-table relationship.

If you have an existing table-to-table relationship, follow the steps below to add lookup fields to the relationship.

To add a Lookup Field by editing an existing table-to-table relationship:
1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Relations. This will display the Table Relations Page

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.4.pngraw=true"><img src="https://github.com/dilip-987/admin-guide/blob/b264631a15503ee6a0d0da14608321cdca7ba9a5/2.4.access-application.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

2.On the Table Relations Page, next to the desired relationship click the edit icon

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.4(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.4(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


3. On the Create Relations Page displayed, click Add Lookup Field button.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.4(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.4(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


4. Click on the drop-down option to select the Lookup Field you wish to add to the child table. 

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.4(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.4(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


5. Continue to add other lookup fields if desired by using the + option. Add/Remove fields by using the +/– options.

6. Once all desired Lookup Fields have been added, click Save Changes.

Once the relationship is updated, the lookup fields will be automatically added to the child table (the table referencing the information from the parent table).

## 3.5 Create Summary Fields
A Summary Field is a field added to the parent table of a relationship to summarize fields from referenced records in the child table. 

For example, a summary field called order count can be added to the customer table (parent table) to count the number of order records where each customer is referenced in the order table (child table). This summary field will thus display the number of orders placed by each customer.

Summary Fields can be added by editing an existing table-to-table relationship. Please refer to the section “Add a Relationship between Tables” if you need to create a table-to-table relationship.
If you have an existing table-to-table relationship, follow the steps below to add summary fields to the relationship.

To add a Summary Field by editing an existing table-to-table relationship:
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Relations. This will display the Table Relations Page.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.5.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.5.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

 
  2. On the Table Relations Page, next to the desired relationship click the edit icon
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.5(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.5(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    3. On the Create Relations Page under Parent Table, click Add Summary Field button.

    4. Enter a Name for the Summary Field and Click on the drop-down option to select the Type of Summary you wish to add to the parent table.

The Summary type can be a count of the related records in the child table, or can be the summary of any specified field in the child table.
If the summary type chosen is Summary of a specific field, you will have to select the following from the drop-down options:

    • A Field to Summarize (Column from the child table you wish to summarize) 
    • The Aggregate Function (Sum, Average, Min, Max)

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.5(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.5(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


For example, the Summary of a specific field could be the Sum of the dollar amount field from the child table “order”. The summary field will display the total dollar amount for each customer record in the parent table “customer”.

    5. Save Changes when done.

    6. At this point you can add other summary fields if needed by repeating above steps 3-5.

    7. Click Save Changes to update the Relationship when done.
Once the relationship is updated, the summary fields will be automatically added to the parent table.

## 3.6 Import Data into a Table

The Import Data feature is available to import data into an existing table that contains fields which correspond to the data to be imported. There are a few methods available to import data which include specifying a URL address that points to either a CSV file or a resource that will return a JSON dataset.

To import data into a table:
 1. First, ensure that the table to which you are importing data contains all the required fields to hold the data.

 2. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Import Data. This will display the Import Data Page.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


3. Click Create Import at the upper-right corner of the page. 

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

4. On the next screen displayed, select an Import Type from the drop-down option, and follow the steps below based on the import type selected.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


The following import types are available:

    • CSV File	:	To easily upload a CSV File
    • CSV Endpoint	:	To pull data from a public URL that points to a CSV File. This can also 
be used to import data from one table to another.	
    • JSON		:	To pull data from a public URL that points to a JSON Dataset
    • MsSql		:	To pull data from a database


    A. To import a CSV File from your computer:

    • Select CSV File from the drop-down, then Click on Choose File to select a CSV file from your computer.


<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    B. To import a CSV from a URL:

    • Select CSV Endpoint from the drop-down, then enter the URL address of the location containing the CSV file and click Import CSV.


<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(4).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(4).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



Note: A Dropbox File link can also be used with CSV Endpoint to import data from a CSV file in Dropbox. The URL address will be the File Link in Dropbox.

Enter the File Link from Dropbox, then set the last part of the link from dl=0 to dl=1 (example: https://www.dropbox.com/s/../ImportFile.csv?dl=1). 

To get the File link in Dropbox, simply click Share > Create Link > Copy Link.


    C. To import a JSON data set: 

    • Select JSON from the drop-down, then enter the URL address of the resource (API) location that will return the JSON data set and click Import JSON.


<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(5).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(5).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    D. To import data from a database: 

    • Select Database from the drop-down, then enter the Connection Parameters for the specific database which include the database, server, username and Password. Click Connect when all the credentials are entered.


<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(6).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(6).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


 5. Once the import step is complete, the Field Mapping screen will be displayed. 

 6. On the Field mapping screen, under the Import Type Section: 

You will have the option to merge in records from the file to the table. The merge option will update the records that already exist in the table, and will add any new records to the table.

To merge records, select the Merge Key Field (the primary field in the table used as the unique identifier such as Order Number), and select a Source Field (the field in your data that corresponds to the Merge Key Field specified).

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(7).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(7).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

7. On the Field mapping screen, under the Filter Data Section: 

You will be able to filter the data you wish to import. To filter data, select a desired Column (field from your data), a Condition (for example “is equal to”), and enter the Value you wish to filter.
Use the +/- Action buttons to add or remove criteria.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(8).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(8).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



8. On the Field mapping screen, under the Field Mapping Section:
You will map the fields from your data (Source Fields) to the fields/columns in your table. 

For each source field you will have the following mapping options:

    A. To Existing Field – if you wish to Map to an Existing Field in your Table:

    • Select the To Existing Field option and click on the drop-down to select the field on your table you wish to map the source field to.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(9).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(9).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    B. Do Not import - if you do not wish to import a specific column from your data:

    • Simply select the Do Not Import option. The data from the source field will not be imported.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(10).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(10).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    C. Create a New Field – if you wish to create a new field in order to import a field that currently does not exist in your table:

    • Click Create New Field and enter a Field Name and Field Type on the screen displayed, then click Save Changes.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(11).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(11).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(12).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(12).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


9. Continue to map all source fields as needed. Once the Field mapping has been completed, scroll down and click Next at the bottom right.

10. A. If importing data from a CSV File:

    • Click Save Changes on the next screen. The import should be complete at this point, and the data should now be imported to your table.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(13).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(13).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


B. If importing data from a CSV Endpoint URL, JSON URL, or Database:
You will have the option to create a data refresh schedule, and a purge schedule. 

A data refresh can be scheduled to automatically import data from the import location into your tables. This will ensure that your data is automatically updated regularly rather than you having to manually refresh the data.

A purge schedule can be set up to regularly delete records from your tables. For example, a purge schedule can be set up to delete records older than 10 days.

If you do not wish to create a Refresh and Purge Schedule click Next, then click Save Changes. The import is complete at this point, and the data should now be imported to your table.

Note: Refresh and Purge schedules can be added to existing imports at a later time.

Note: Refresh and Purge schedules can be added to existing imports at a later time.

    • On the Schedule Screen, enter a Name for the Schedule, a Description, a Frequency (Minutes, Hours, Days, Weeks, Months, Years), and an Amount for the frequency (the interval of time or rate at which the data refresh needs to occur). For example, for a frequency of 30 minutes: the data would be pulled from the Import location every 30 minutes.

    • Click Next to proceed to the next screen (Purge Schedule screen).

    • If you do not wish to add a purge schedule, click Save Changes. At this point the import would be complete, the data would be added to your table and the refresh would be set.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(14).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(14).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


If you wish to add a Purge Schedule, follow these steps:
    • On the Purge Screen, enter a Name for the Purge, a Description, a Frequency (Minutes, Hours, Days, Weeks, Months, Years), and an Amount for the frequency (the interval of time or rate at which the data purge needs to occur). For example, for a frequency of 7 days: the data would be purged from the table every 7 days.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(15).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(15).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    • Under Filter data, enter the criteria that specify which records need to be deleted. To filter data, select All or Any (to specify whether All or Any one of the filter conditions need be true). 

    • Next, select a desired Column (field from your table), a Condition (for example “is equal to”), and enter the Value you wish to filter.

    • Use the +/- Action buttons to add or remove criteria.

    • Click Save Changes when done. At this point the import would be complete, the data would be added to your table, and the refresh and purge schedules would be set.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(16).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.6(16).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


## 3.7 Manage a data refresh
 
A data refresh can be scheduled to automatically import data into your tables. This will ensure that your data is automatically updated regularly rather than you having to manually import the data. The data refresh can import data from the following:
    • A CSV Endpoint (CSV URL)
    • A JSON Dataset
    • A Database

### 3.7.1 Schedule a Data Refresh (if not previously created with a data import)

A data refresh can be created while setting up a data import or at any point after that.

The data refresh is added to existing data imports that you previously created. To create data imports, please refer to the section “Import Data into a Table”. You will be able to create a refresh schedule for CSV Endpoint, JSON and Database Import Types.

Note: Multiple Data Refresh schedules can be created at any time. Simply follow the steps outlined in this section to add your schedules.

1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Import Data. This will display the Import Data Page.
 <a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.1.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


 2. On the Import Data Page, locate the Import you wish to add a refresh schedule to and click the schedule icon next to the import.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.1(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.1(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



 3. On the next screen displayed, click Add Schedule.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.1(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.1(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


4. On the Entry screen displayed, enter a Name for the Schedule, a Description, a Frequency (Minutes, Hours, Days, Weeks, Months, Years), and an Amount for the frequency (the interval of time or rate at which the data refresh needs to occur). For example, for a frequency of 30 minutes: the data would be pulled from the Import location every 30 minutes.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.1(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.1(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



5. Click Save Changes.

6. If needed to add another schedule, click Add Schedule once more and repeat steps 4-5.

### 3.7.2 Delete a data refresh schedule
 
To Delete an existing Schedule: 
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Import Data. This will display the Import Data Page
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.2.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.2.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    2. Click the Schedule icon  next to the desired data import record. This will display the Schedule Page for that data import. 

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.2(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.2(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. Click the X icon next to the desired schedule to remove it.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.2(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.2(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    4. Click OK to on the screen displayed to confirm.

### 3.7.3 Manually refresh data in a table
You will be able to manually refresh data for existing Imports with CSV Endpoint, JSON and Database Import Types.

To Manually Refresh Data in a Table: 
 1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Import Data. This will display the Import Data Page.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.3.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.3.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


2. Click the Reload icon  next to the desired data import record.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.3(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.7.3(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

3. Click OK to confirm the reload. The data should now be updated in your table.

## 3.8 Deleting and Editing table elements

Tables and Table elements – including fields and relationships – can be deleted and edited at any point from the application. The following subsections describe how to delete/edit fields, relationships, and tables.

### 3.8.1 Delete/Edit a Field from a Table

1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Fields.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.1.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    2. On the Fields Page displayed, locate the field you wish to delete, and click the X icon next to the field.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.1(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.1(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. On the pop-up window displayed, click OK to confirm.

To Edit a Field Name on a Table: 
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Fields.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.1(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.1(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    2. On the Fields Page displayed, locate the field you wish to edit, and click the Edit Icon next to the field.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.1(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.1(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. On the pop-up window displayed, update the Field Name and update the “Must be unique” flag if needed. Click Save Changes when done.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.1(4).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.1(4).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


### 3.8.2 Delete or Edit a relationship

To Delete a Relationship between Tables: 
  1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Relations.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.2.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.2.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

2. On the Relations Page displayed, locate the relationship you wish to delete, and click the X icon next to the relation.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.2(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.2(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


3. On the pop-up window displayed, click OK to confirm.
To Edit a Relationship between Tables: 
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Relations.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.2(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.2(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    2. On the Relations Page displayed, locate the relationship you wish to edit, and click the Edit icon next to the relation.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.2(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.2(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. On the Create Relations Page displayed, update the relationship as needed and click Save once done.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.2(4).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.2(4).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


### 3.8.3 Delete an Entire Table or Edit a Table Name

To Delete an entire Table: 
    1. Access the Application’s Tables Page.

    2. On the Tables Page, locate the table you wish to delete, and click the X icon next to the table.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.3.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.3.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. On the pop-up window displayed, click OK to confirm.
    
    To Edit a Table Name:
    1. Access the Application’s Tables Page.

    2. On the Tables Page, locate the table you wish to edit, and click the Edit icon next to the table.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.3(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.8.3(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. On the pop-up window displayed, update the Table Name and click Save Changes when done.

## 3.9 Viewing a Table and its Data

A table and its data can be easily displayed from the application. The View Table function will allow you to view the fields and data in a table. This will display the default report if any (this is discussed in the Manage Reports Section), otherwise this will display the unfiltered table’s data with the max number of records specified.

To View a Table:
1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click View Table.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.9.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.9.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

2. This will display the Default Report created for that table if any. If there is no default report, this will display the table’s unfiltered data with the max number of records specified.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.9(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.9(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


To Export Data:
    1. On the View Table Page, click on the desired buttons to Copy or Export data:

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.9(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.9(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    A. Copy to copy the data in order to paste on a desired document
    B. CSV to export a CSV File
    C. Excel to export the data to an Excel File
    D. PDF to export the data into a PDF
    E. Print to print the data

## 3.10 Create and Manage Reports

Reports are used to view/display data from your tables. Reports can be easily created in the application. When creating a report, you can specify/filter the data you want to see based on specific values, and order the data as desired.

You can create the following types of report formats:
    • Table		:	Displays specific records from your data
    • Charts		:	Creates a graphical representation of the desired data
    • Summary	:	Summarizes your data with sums, averages and other statistics 

### 3.10.1 Add Reports

To Add a Report:
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Reports. This will display the Table’s Reports Page.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    2. On the Table’s Reports Page, click Add Report at the upper-right corner.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. At this point, you will have the option to create a tabular report, a chart or a summary report. Follow the steps for the desired option.
To Create a Tabular Report:
    1. On the Select Report window displayed, select Table.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    2. On the Create Reports Page, under Reports Fields:

Enter a Report Name, and Description (Optional). 

    • Select the Check as Default checkbox if you wish the report to be your primary/default report to appear when you select/view the table.
    • Select the Global checkbox to allow all users to view the report. The users will not be allowed to edit the report.
    • Select the Public checkbox to allow the data in the report to be available to other tables. This will allow using a CSV endpoint for table to table imports.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. On the Create Relations Page, under Columns:

Select the Fields/Columns you wish to view on the report. Use the arrows to add/remove fields to/from the report.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(4).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(4).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    4. On the Create Relations Page, under Filters:

If desired, you will be able to filter the data you wish to view on the report:

First, select All or Any to specify whether All or Any one of the filter conditions need be true. You will then select a desired Column (field from your table), a Condition (for example “is equal to”), and then enter the Value you wish to filter.

Use the +/- Action buttons to add or remove filter criteria.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(5).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(5).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


The group of filter criteria allows you to specify that either All or Any of the conditions need to be true within that group. If you have additional groups of criteria, you will be able to add nested groups (i.e. additional groups of filter criteria). This will allow you to use different combinations of the All or Any options. 

For example, the filter criteria can be: [Customer State is FL OR GA], AND [Dollar Spent is greater than $1,000 AND Number of Orders is greater than 10]. In this case, two groups of filter criteria would be used as shown in below screenshot.

To add an additional nested group, click Add Group at the top right of the Filters Section

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(6).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(6).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>




Note: To remove a nested group you no longer need, simply click on the X Icon next to the group.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(7).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(7).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    5. On the Create Relations Page, under Sorting:

You will be able to sort/order the records on your table based on the specified criteria:

Select a Sort Type (Low to High or High to Low), and select the Sort Field (the field you wish to sort the report by).
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(8).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(8).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    6. Click Save Report when done.

To create a Summary Report:
    1. Follow the first steps to add a report as described in previous “To Add a Report” Sub-section. 

    2. On the Add Report Window displayed, select Summary.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(9).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(9).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    3. On the Create Reports Page displayed, enter a Report Name. Select the Global checkbox if desired. The Global setting will allow all users to view the report. The users will not be allowed to edit the report.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(10).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(10).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    4. On the second half of the Page, click on the Fields Icon on the right. This will display the Fields Window.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(11).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(11).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    5. On the Fields Window, select and drag the desired fields to the desired section on the right of the window (described below). 
Note: Some of the fields might already be pre-loaded under a section, update them as needed onto the following sections:

    • Report Filters:Under Report Filter, drag and drop any field you would like to use to filter the data. This will add a filter to the report that will allow selecting values when the report is displayed.

    • Rows:
Under Rows, drag and drop the field(s) that will represent the rows on your report.

    • Columns:
The Values Field will be pre-loaded under Columns. The Values Field represent the values that will be calculated based on your selection. As a default, these values are displayed across a column
You can drag and drop any additional field(s) that will represent the columns on your report and if you would like to further break down the columns in your report. 

    • Values:
Under Values, drag and drop the Values field(s) that need to be summarized. Once a field is added, click on the Sum icon next to the field, to select what function is to be performed on the value (i.e. Sum, Count, Average etc...)

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(12).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(12).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    • Calculated Values:
A custom formula can also be added to the report if the summary values are not sufficient. Click on the Add Calculated value button at the top. 

On the window displayed, enter the formula name, then enter the desired formula by selecting the fields and operations to be used within the formula. 
Click Apply when done.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(13).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(13).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


Example of a summary Report:

A summary report can be used to display the total number of units ordered by item category broken down by item. In addition, the report can also have a filter to allow selecting specific orders. The following steps will be taken:

1) To filter the report by order, the order field is dragged onto the Report Filter Section.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(14).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(14).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



2) The report will be broken by item category first and then by item. To display these fields as rows, they will be dragged onto the Rows Section (the item category field first followed by the item field).

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(15).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(15).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


3) The report will sum the total number of units ordered. The Quantity field will thus be dragged onto the Values Section and the function Sum will be selected.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(16).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(16).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


4) Under Columns, the Values Field represent the values that will be calculated based on the selection (i.e. the Sum of the Quantity). In this case, the Calculated Values will be displayed across a column.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(17).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(17).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    6. When the report is displayed, you can filter the report if needed by clicking on the filter options displayed on the report (any field with the Tools Icon  can be filtered). Click on the field that needs to be filtered. On the Filter window displayed, Select/Unselect the desired values and click Apply when done.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(18).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(18).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    7. In addition, you can also use the filter option to filter the Variables or Values by specific conditions. On the Filter Window:
    • To filter the variables, click Labels and enter your filter criteria.
    • To filter the values, click Values and enter your filter criteria.
    • To sort the data, click AZ to Sort Ascending or ZA to Sort Descending.
Click Apply when done.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(19).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(19).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    8. When the report is displayed, you can also format the cells as desired. To format the cells, click on the Format Icon at the top right of the report. 

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(20).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(20).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    9. Click Save Report when done.

To create a Chart:
  1. Follow the first steps to add a report as described in previous “To Add a Report” Sub-section.
  2. On the Add Report Window displayed, select Chart.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(21).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(21).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

3. On the Create Reports Page, Enter a Report Name. Select the Global checkbox if desired to allow all users to view the report. The users will not be allowed to edit the report

4. On the Create Reports Page, select the Chart Type you wish to create. Note: A report might be pre-loaded on the second half of the screen, however you will be able to update the details as needed.

5. After you select the Chart Type, click on the Fields Icon at the top of the report that is displayed on the second half of the page.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(22).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(22).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


 6. On the Fields Window, select and drag the desired fields to the desired section (described below). 
Note: Some of the fields might already be pre-loaded under a section; update them as needed onto the following sections:

    • Report Filters:
Under Report Filter, drag and drop any field you would like to use to filter the data. This will add a filter to the report that will allow selecting values when the report is displayed.

    • Rows:
Under Rows, drag and drop the field(s) that will represent the variables or categories on your report.

    • Columns:
The Columns represent the values that will need to be compared across the variables/categories on your report. The Values Field will be pre-loaded under Columns. 

You can drag and drop any additional field(s) to further break down the values in your report. 

    • Values:
Under Values, drag and drop the Values field(s) that need to be compared on your report. Once a field is added, click on the Sum icon next to the field, to select what function is to be performed on the value (i.e. Sum, Count, Average etc...)

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(23).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(23).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    • Calculated Values:
A custom formula can also be added to the report if the summary values are not sufficient. Click on the Add Calculated value button at the top. 

On the window displayed, enter the formula name, then enter the desired formula by selecting the fields and operations to be used within the formula. 
Click Apply when done.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(24).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(24).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



	Example of a Chart Report:

A Chart report can be used to display the distribution of sales in dollar amount by department. A Pie Chart can be used to represent the total dollar amount ordered for each category. 
In addition, the report can also have a filter to allow selecting specific orders. The following steps will be taken:

1) To filter the report by order, the order field is dragged onto the Report Filter Section.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(25).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(25).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


2) The report will be broken by item category. The item category field will be dragged onto the Rows Section to represent the variable/category of the report.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(26).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(26).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


3) The report will sum the total dollar amount sold for each item category. The Dollar field will thus be dragged onto the Values Section and the function Sum will be selected.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(27).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(27).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


4) Under Columns, the Values Field represent the values that will be calculated based on the selection (i.e. the Sum of the Dollar Amount). In this case, the Calculated Values will be displayed for each variable.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(28).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(28).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    7. When the report is displayed, you can filter the report if needed by clicking on the filter options displayed at the top right of the report. On the Filter window displayed, select/Unselect the desired values on the Filter window and click Apply when done.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(29).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(29).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    8. In addition, you can also use the filter option to filter the Variables or Values by specific conditions. On the Filter Window:
    • To filter the variables, click Labels and enter your filter criteria.
    • To filter the values, click Values and enter your filter criteria.
    • To sort the data, click AZ to Sort Ascending or ZA to Sort Descending.
Click Apply when done.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(30).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(30).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    9. When the report is displayed, you can also format the report fields as desired. To format the fields/values, click on the Format Icon at the top right of the report. 

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(31).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.1(31).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    10. Click Save Report when done.

### 3.10.2 Set an existing report as default for a table

When a Report is set as the default report of a table, that report will be automatically displayed when a user views a table (i.e. when a user selects the View Table option). If a table does not have a default report, the table’s unfiltered data is displayed instead when a user views the table.

To set a Table’s Default Report:
  1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Table Settings.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.2.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.2.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



 2. On the Table Settings Page, next to Default Report, select a report from the drop-down menu. This report will then be automatically displayed when a user views the table.

### 3.10.3 Display Default Reports

To view/display a Default Report:
  1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click View Table

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.3.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.3.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

2. This will display the Default Report created for that table if any. If there is no default report, this will display the table’s unfiltered data with the max number of records specified.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.3(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.3(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


### 3.10.4

To Delete a Report: 
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Report.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.4.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.4.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    2. On the Reports Page displayed, locate the report you wish to delete, and click the X icon next to the report.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.4(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.4(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. On the pop-up window displayed, click OK to confirm.

To Edit a Report: 
   1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Report.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.4(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.4(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


 2. On the Reports Page displayed, locate the report you wish to edit, and click the Edit icon next to the report.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.4(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.10.4(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

3. On the next page, make the desired changes, and click Add Report to update the report.


## 3.11 Create and Manage Forms

Data Entry Forms are used to manually add records to a table as well as to manually edit existing records on a table. Data Entry Forms can be easily created in the application, as well as Mobile-Friendly Forms. 

Note: Data entry forms will be associated with Reports when the forms are being created. With this, you will be able to see the form in order to add or edit records when viewing a report.

Since forms are linked to reports when forms are being created, reports will have to be created prior to creating data entry forms. 

To Add a Form:

Make sure a report has been creating prior to adding a form. See Add Reports Section on how to create reports.
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Forms. This will display the Table’s Forms Page.

    2. On the Table’s Forms Page, click Add Form at the upper-right corner.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    3. On the Create Form Page, under Fields:

    • Drag and Drop to add fields to a row of the form. These will be the fields for which you wish to be able to add/edit data manually.

    • Insert/remove rows with the plus/minus buttons, if you wish to have multiple rows displayed on the form.
Once the Fields are added, select the “Required” Flag next to each field if a value is required for that field when adding records to a report.
<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    • In addition, if you prefer to have multiple tabs on your forms, click on Add Tab. With multiple tabs, you can set the fields to be displayed on different tabs of the form rather than displayed to the user all at once on one tab.

If you add multiple tabs, update the tab’s title. 

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    4. Click Add Form when done.

### 3.11.2 Add Mobile Forms
Mobile Forms are used to edit/add data on a mobile or add Form via the Mobile App.

To Add a Mobile Form:
                            1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Forms. This will display the Table Forms Page.

                            2. On the Table Forms Page, click the Mobile Form Icon at the upper-right corner.


### 3.11.3 Edit or Delete Forms


To Delete a Report: 
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Forms.

    2. On the Forms Page displayed, locate the report you wish to delete, and click the X icon next to the report

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.3.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.3.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    3. On the pop-up window displayed, click OK to confirm. 

To Edit a Form:
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Forms.

    2. On the Forms Page displayed, locate the form you wish to edit, and click the Edit icon next to the report.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.3(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.3(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    3. On the next page, make the desired changes, and click Add Form to update the form.

### 3.11.4 Manually Add or Edit Records

Once a data entry form has been created, records can be easily added to the report the form was assigned to. Records can also be edited.

Note: To be able to add or edit records, a data entry form must be created and associated with the report. Otherwise, the Edit and Add Record options will not be available on the screen.

To Manually Add Records to a Table: 
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click View Table. 

    2. On the View Table Page displayed, click the Add button at the top right of the page.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


    3. On the Data Entry form, enter the values you wish to add for each field of the form. 

If you have any relations created for the table, you may notice some drop-down fields which represent the reference fields from the parent table. 
Simply click on the drop-down option to select a value for these fields.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    4. Click Save when done.

To Manually Edit Records in a table: 
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click View Table.

    2. On the View Table Page displayed, locate the record you wish to edit, click the Edit Icon next to the record. This will pull up the data entry form associated with the default report.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. On the Data Entry form, enter the values you wish to update for each field of the form. 

If you have any relations created for the table, you may notice some drop-down fields which represent the reference fields from the parent table. 
Simply click on the drop-down option to select a value for these fields.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    4. Click Save when done.

To Manually Add Records to a Table through a Report: 
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Reports.

    2. On the Reports Page displayed, locate a Report that contains all the required fields for your table. 
Click on the View Report icon. This should display the report and its records.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(4).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(4).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. On the report displayed, Click the Add Record button at the top right of the screen. This will pull up the Data Entry Form associated with the report.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(5).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(5).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    4. On the Data Entry form, enter the values you wish to update for each field of the form. 

If you have any relations created for the table, you may notice some drop-down fields which represent the reference fields from the parent table. 
Simply click on the drop-down option to select a value for these fields.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(6).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(6).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    5. Click Save when done.

To Manually Edit Records in a table through a Report: 
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Reports.

    2. On the Reports Page displayed, locate the Report that contains the records you wish to edit, and click on the View Report icon. 
This should display the report and its records.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(7).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(7).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    3. On the report displayed, locate the record you wish to edit, click the Edit Icon. This will pull up the data entry form associated with the report.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(8).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(8).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

   4. On the Data Entry form, enter the values you wish to update for each field of the form.

If you have any relations created for the table, you may notice some drop-down fields which represent the reference fields from the parent table. 
Simply click on the drop-down option to select a value for these fields.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(9).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.4(9).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    5. Click Save when done.


### 3.11.5 Manually Delete RecordsTo Manually Delete Records from a table: 
    1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click View Table.

    2. On the View Table Page displayed, locate the record you wish to delete, click the Delete Icon next to the record.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.5.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.5.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



    3. Click OK on the Delete Record screen displayed.

To Manually Delete Records from a Table through a report: 
   1. On the sidebar menu, click on the drop-down arrow next to the desired table, and click Manage Reports.

   2. On the Reports Page displayed, locate the Report that contains the records you wish to edit, and click on the View Report icon. 
This should display the report and its records.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.5(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.5(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

3. On the report displayed, locate the record you wish to delete, click the Delete Icon. 
 <a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.5(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/3.11.5(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

4. Click OK on the Delete Record screen displayed.


# Chapter 4 – Custom Pages

## 4.1 Managing Custom Pages

A Custom Page is used to create a Home Page for users of the application. The custom page will be able to display any type of information with custom views. This can serve as a customized home page or dashboard page with any information or tools including reports, data, entry forms, external links etc.…

The Custom Page is an HTML Page. You can enter any HTML Code to create the page, and you will be able to use the API to create custom views. Please refer to the Ignatius API Documentation for instructions on using API Commands to add, modify, delete, or query tables, reports, charts, fields, forms, relations, and notifications within the database.

To add a Custom Page:
 
1. On the sidebar menu, click Pages to access the custom pages of the application.


<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1.png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

                                                 2. On the Custom Pages Page displayed, click Add Page. This will display a screen where you will be able to enter the HTML Code for your page.


<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(1).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


                                                 3. On the Screen displayed, enter the HTML Code for your page. Please refer to the Ignatius API Documentation for instructions on using API Commands.


<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(2).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



4. Select the Default Page checkbox if you wish this page to be the default home page that users see when they log in to the application.

5. Click Save Changes when done. If the Default Page checkbox was selected, users will see this page the next time they log in to the application.

To edit a Custom Page:
1. On the sidebar menu, click Pages to access the custom pages of the application.


<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(3).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    2. On the Custom Pages Page displayed, click the Edit Icon next to the page you wish to edit. 

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(4).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(4).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    3. On the Screen displayed, make the desired updated to your page. Please refer to the Ignatius API Documentation for instructions on using API Commands.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(5).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(5).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    4. Click Save Changes when done. If the Default Page checkbox was selected, users will see this page the next time they log in to the application.

To delete a Custom Page:
    1. On the sidebar menu, click Pages to access the custom pages of the application.


<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(6).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(6).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    2. On the Custom Pages Page displayed, click the Delete Icon next to the page you wish to edit.


<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(7).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(7).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    3. Click OK to confirm.

To add a Default Custom Page to an Application:
    1. On the sidebar menu, click App Settings.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(8).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(8).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    2. On the App Settings Page displayed, select the View Settings Tab.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(9).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.1(9).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>
    3. From the Default Page drop-down option, select the custom page that you wish to be set up as the Default page for the Application.


## 4.2 Assigning Custom Pages to Tables

In addition to custom pages being set up as the Home Page or Dashboard seen by users log into the application, custom pages can also be linked to tables. The custom page linked to a table will be the page displayed when a user selects that table in the Application.  

To set up an existing custom page for a table:
1 On the sidebar menu, click Pages to access the custom pages of the application.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.2.png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.2.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    2. On the Custom Pages Page displayed, locate the custom page you wish to set up as the Table’s Home page. Click the Settings Icon next to the page. 

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.2(1).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.2(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    3. On the window display, select the table(s) you wish to map the custom page to.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.2(2).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.2(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    4. Click Save Changes when done. The custom page will be displayed the next time a user clicks on the table.

To display the home page of a table:

    1. On the sidebar menu, click on the desired Table. 

If a custom page is linked to the table, the custom page will be displayed.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.2(3).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/4.2(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

# Chapter 5 – Manage user roles and permissions

This chapter will go over how to create/manage users and user roles. A user is anyone who logs into or uses the application. A user can be an Admin User or a Non-Admin/Regular User. 

Admin users are the users who will set up and configure the application including managing and creating tables, reports, forms etc... Admin users will have the highest level of permissions and will be able to perform any task from creating tables to creating new users to managing the application’s settings.

Non-Admin users are users who will access the application to simply manage the data which includes viewing, editing or adding records. Non-Admin users are assigned a user role that will define their level of access and required permissions. 

A user role represents a user’s permissions which includes the tables the user has access to as well as the actions (add/delete/update records etc.…) a user is allowed to perform.

Note: A user role must be created prior to creating a new non-admin user if the desired user role for that user does not yet exist.

## 5.1 Adding a User Role

The user role dictates which tables a user will have access to, as well as which actions a user will be able to perform. Any existing user role can be assigned to multiple users.

To add a User Role to an application:

    1. On the sidebar menu, click App Settings to access the Settings Page.
<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.1.png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    2. On the App Settings Page displayed, click on the Roles tab. 

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.1(1).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.1(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    3. On the Roles tab, click Add Role.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.1(2).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.1(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    4. Enter a Name for the User Role, and select an Application Default Page from the drop-down option. This will be the Custom Page the users with that user role will see when logged in.

    5. Next, for each of the tables displayed, select all the required options/permissions for the role. The following options can be selected:

    • View			: 	To view records on a table
    • Edit			:	To change records on a table
    • Add			:	To add records/data to a table
    • Delete			:	To delete records from a table
    • Default Page		:	The custom page this user role will see when selecting a table


<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.1(3).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.1(3).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    5. Next, click on the Management Folder next to a table to select the management permissions this user role will have for that particular table. This will display a window from which you can select the following options. These options are usually Admin permissions:

    • Import Data		: 	To import data into the table via CSV File or CSV Endpoint
    • Manage Reports	:	To create, edit, delete reports for the table
    • Manage Forms		:	To create, edit, delete forms for the table
    • Hide Table		:	To hide the table

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.1(4).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.1(4).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    6. Click Save Changes when the Management functions are selected (if needed). 

    7. Click Save on the Roles Page when done. The user role created is now available to assign to new or existing users.

## 5.2 Adding a New User

Admin users are the users who will set up and configure the application including managing and creating tables, reports, forms etc... Admin users will have the highest level of permissions and will be able to perform any task from creating tables to creating new users to managing the application’s settings.

Non-Admin users are users who will access the application to simply manage the data which includes viewing, editing or adding records. Non-Admin users are assigned a user role that will define their level of access and required permissions. 

When creating a new non-admin user, a user role will be assigned to that user’s profile. The desired User Role must exist prior to creating the non-admin user. Refer to the Adding a User Role Section for details on how to create a user role.

To add a User to an application:

   1. On the sidebar menu, click App Settings to access the Settings Page.


<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.2.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.2.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


   2. On the App Settings Page displayed, under the Users Tab click Invite User.

<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.2(1).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.2(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

   3. On the window displayed, enter the user’s email address.

   4. Next select the following depending on whether the user is Admin or Non-Admin:
    • If the user being created is an Admin user, select the Is Admin checkbox
    • If the user being created is a Non-Admin user, select a User Role from the drop-down option 


<a href="https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.2(2).png?raw=true"><img src="
https://github.com/dilip-987/admin-guide/blob/aef2ab45878184016f100657b67e1166edcec205/5.2(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

   5. Click Save when done. The user will receive an email at the specified email address, and will be able to create a password and log into the application.

# Chapter 6 – Create workflows and notifications 

## 6.1 Adding Notifications

Notifications can be sent to alert you when records have been changed on a specific table. Notifications can be set to alert you when new records have been added to a table, when records have been updated, and when records have been deleted from a table. 

Notifications are used to help you keep track of the changes happening in the application. Notifications are set up at the table level, so you will be able to set up notifications for each table in the application if desired. 

To add Notification for a Table:
   1. On the sidebar menu, click Manage Notifications under the table for which you wish to add a notification.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/6.1.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/6.1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

   2. On the Notifications Page displayed, click Add Notification.

   3. On the Create Notifications Page displayed, under the Notification Fields: 

    • Select a Notification Type, and enter the recipient’s information
        ◦ SMS	: 	To alert via Text Message
        ◦ Email	: 	To alert via Email
        ◦ Facebook	:	To alert via Facebook message

    • Enter a Subject line for the Notification message

    • Select a Trigger Type (New Record, or Update Record). 
The trigger type is the activity (record change) for which you wish to send a notification. 

For example, if you wish to send a notification for the Customer table when a record is updated on the table, the trigger type in this case would be Update Record.

    • Under Fields, select the desired option. If the option “Any of the following fields affected by trigger event” is selected, then the table’s field will be displayed. Select the fields for which you wish to set up the notification.

    • Under Sent to All Users, select Yes or No. If ‘Yes’ is selected, all users will receive the Notification. If ‘No’ is selected, this will display a field where you will enter the users who need to receive the notification.

    • For the Notification Message, you can do one of the following:

        A. Select the Custom option if you wish to send a custom alert message. If this option is selected, enter the custom message that needs to be sent.

        B. Select the Value in Field option to send a default message specifying the record that was changed. 
From the drop-down option, select the field whose value you wish to be included in the notification message. 
For example, if a record was updated on the Customer Table, and the field selected was Last Name, then the alert message will include the last name of the customer record that was updated. 

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/6.1(1).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/6.1(1).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


4. On the Notifications Page displayed, under Filters: 
You will be able to filter the data for which notifications are set. For example, if you would like alert messages to be sent when a record is changed for a specific customer, you will be able to specify the customer’s information as filter criteria.
    • To filter data, select All or Any (to specify whether All or Any one of the filter conditions need be true). 

    • Next, select a desired Column (field from your table), a Condition (for example “is equal to”), and enter the Value you wish to filter.

    • Use the +/- Action buttons to add or remove criteria.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/6.1(2).png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/6.1(2).png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



  5. When done, click Add Notification to create the notification.

# Chapter 7 – Power BI Reports
Power BI is a business analytics service that is integrated with Ignatius. Power BI is available to provide interactive visualizations and business intelligence capabilities that users can use to create reports and dashboards.

## 7.1 Loading Reports

To load a Report from Power BI:
    1. On the sidebar menu, click Power BI Reports to access the reports.

<a href="https://raw.githubusercontent.com/dilip-987/admin-guide/008c03a51fa6621dac9d8987b1ba48d6b26770a4/7.1.1.png"><img src="https://raw.githubusercontent.com/dilip-987/admin-guide/008c03a51fa6621dac9d8987b1ba48d6b26770a4/7.1.1.png" width="550" alt="n8n.io - Screenshot"></a>


    2. On the Power BI Reports Page displayed, select a Report/Dashboard from the drop-down option. Then select whether you wish to View or Edit the report.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/7.1(1).png"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/7.1(1).png" width="550" alt="n8n.io - Screenshot"></a>



    3. Click Load Report. The Power BI Report will be displayed at the bottom of the page.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/7.1(2).png"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/7.1(2).png" width="550" alt="n8n.io - Screenshot"></a>


<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/7.1(3).png"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/7.1(3).png" width="550" alt="n8n.io - Screenshot"></a>



    4. Use the tabs at the bottom of the loaded report/dashboard to navigate through the different reports if any.

<a href="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/7.1(4).png"><img src="https://github.com/dilip-987/admin-guide/blob/a0bf27a9f3e93b13f1c71ff98f6b8d5fde9c843a/7.1(4).png" width="550" alt="n8n.io - Screenshot"></a>



# Chapter 8 – Audit Log

The Audit Log Feature will display a log of all the activities that occurred within the tables of the application. The logs will display records that have been added to tables and modified.

## 8.1 Viewing the Audit Log

To view the Audit Log:
    1. On the sidebar menu, click Audit Log.

<a href="https://github.com/dilip-987/admin-guide/blob/f415ac1bd950e85bb51bbe0ceb5675904ae77e66/8.1.1.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/f415ac1bd950e85bb51bbe0ceb5675904ae77e66/8.1.1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

    2. Under the Audit Log folder, select View Table. This will display the Audit Log Table with the records of the activities.

<a href="https://github.com/dilip-987/admin-guide/blob/master/8.2.1.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/master/8.2.1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

The Audit Log Table will display the following fields:

    • Field		:	The Field that was updated
    • Value		:	The Value that was inserted into the table
    • Old Value		:	The Value that was in the table prior to the update if any
    • Record ID		:	Unique Identifier for the record
    • Table		:	The Table that was updated
    • Time		:	The time at which the update was done
    • Transaction Type	:	The type of change (i.e. Data Inserted/Data Updated…)

# Adding Formula Fields to a Table

Most fields in a table consist of constant values (either text, numeric, currency, or date). These
values can only be updated manually by editing, or by importing from an external source.
However, there is another type of field based on formulas, that allow you to enter a function
for a data column. This function provides an output for that column based on other field type
values in the same row.
For example, if you create a field called “Average” with the formula: ([num1] + [num2] +
[num3])/3, the data for that column will be the average value for three numeric fields in each
row.
There are four types of formula fields: Text, Numeric, Currency, and Date. For text-based
formulas, you can manipulate values of each data type in various ways to create a customized
or formatted output.
To create a formula field, click the drop-down for the table in which you want to add a formula
field. Then as you click the Manage Fields menu item as shown, a screen will open listing all the
fields currently used for that table.

<a href="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-1.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-1.png?raw=true" width="550" alt="n8n.io - Screenshot"></a> 

Then click the Add Field button in the upper-right corner as explained in section 3.2 to add a
formula field. A pop-up window will open where you can enter the Field Name and Field Type.
We’ll type in “Average” as the Field Name in this example. Then as the drop-down for Field
Type is opened, we’ll select “Formula – Numeric” as shown.

<a herf="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-2.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-2.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

A new text area called “Formula” will then appear in the pop-up where you can enter in the
numeric formula you would like to use. (Example formulas are listed in the next section.)

Other fields are listed on the right that you can use as parameters in the formula. You can just
double-click on one to add it to the formula.

<a herf="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-3.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-3.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>

After the formula is set up, click the Save Changes button to close the pop-up window. The new
formula field should appear in the listing.


<a herf="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-4.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-4.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


<a herf="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-5.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-5.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


You can add more formula fields simply by repeating the steps above.
To see how this function works, switch to View Table in the menu (assuming you have a default
table set up). Edit the table as necessary to get the relevant fields to show up. Make sure you
have a form added in the Manage Forms page to enable editing for numeric values.
Then click Add in the upper-right corner of the View Table page to add a sample row of data.
Enter in vales for num1, num2, and num3 in the spaces provided, and then click Save.
The table will then show the average for three numeric values as shown below:


<a herf="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-6.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-6.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>


# Formula Types

There are four choices for formula types when adding a new formula field: Formula – Text,
Formula – Numeric, Formula – Currency, and Formula – Date.

<a herf="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-7.png?raw=true"><img src="https://github.com/dilip-987/admin-guide/blob/4136f80b31f91087c7a2876f5b5eda06f4e5b4d2/image-7.png?raw=true" width="550" alt="n8n.io - Screenshot"></a>



Formula – Text is used mostly for text methods that can test, modify, combine, or
manipulate text strings in some way. (This type also works for most math functions, so it's
possible to combine a math operator with a text method in some instances.) An example would
be:
If([text1].IndexOf(" ") > [text1].IndexOf("-"), [text1], [text2])
This formula returns text2 if a space occurs before “-“ in text1. Otherwise, text1 is returned.

Formula - Numeric is generally used for performing math operations or any type of
functionality that involves numbers. (Note that this type can also be used for text methods if
the output is a number.) An example is:
[text1].Length * 2 + 3
This doubles the length of text1 (number of characters) and adds 3.
Formula - Currency uses the same basic math operations and methods as the Formula –
Numeric type, except that it is based on currency instead of real numbers. Since this formula
type is used almost exclusively for financial calculations, certain functions that are logarithmic,
exponential, etc. should not be used for this formula type. Numerical data can be used in the
calculation for multiplication, etc., but text methods are not recommended.

Formula – Date has a unique set of operations where you can calculate the time period
between two dates (TimeSpan) or calculate a new date from a given offset (AddTime). The
numeric output for TimeSpan can be used as a numeric input for other types of formulas. The
date output of AddTime can be used as a date input for the TimeSpan formula. There is also a TODAY()
method that returns the today’s date. This can be used in the TimeSpan or AddTime methods if you
need to return a value relative to today’s date.
The methods and operators for these four formula types are listed and described in the next
four sections:


# Formulas: Text Methods

The 32 text methods listed here are in their basic format that provide a simple text or numeric
output based on text inputs. (The input may also include integer values for positioning within
the text.)
Several text methods can be combined into one complex formula you’re looking for a certain
kind of output. An example is:
[text1].Insert([text1].IndexOfAny([text2].ToCharArray()),[text3])
This formula searches through text1 for the first position of any character of text2, and
inserts text3 at that position.

One of the more useful text formulas is the Format method. For example, it can be used to
create a summary statement for customers:
Format("The customer: {0}, purchased the product: {1}, on {2}. The
shipping address is {3}”,[name],[product],[date],[address])
This method will replace all { } items with the corresponding text objects listed. See
Formulas: Format Method for more details about this method.
The following text methods are grouped according to category:

Calculation Methods – Derives string parameters.

Method Example Description
Length [text1].Length Returns the number of characters in the

current string instance.

Concatenation Methods – Appends two or more strings

Method Example Description
+ [text1] + [text2] Concatenates text with a "+".
Concat Concat([text1],[text2]) Appends one text string to another

Compare Methods – Compares the alphabetical position two strings or substrings,
and returns either -1, 0, or 1 based on the sort order. For Example, if the first string is before
the second string alphabetically, -1 is returned. The Equals method returns either “True” or
“False”.

Method Example Description
Equals [text1].Equals([text2]) Returns "true" if the string instance has
the same value as a second string.
Compare Compare([text1],[text2]) Compares the strings and returns their
relative position in the sort order.

Compare while
ignoring case

Compare([text1],[text2],true) Compares the strings and returns their
relative position in the sort order while
ignoring case.

CompareTo [text1].CompareTo([text2]) Compares the current string instance with
the specified string, and returns their
relative position in the sort order.
Compare(advanced) Compare([text1],3,[text2],7,4,true) Compares the substrings and returns their
relative position in the sort order. The
starting point of the comparison is given
by the first two integers, while the third
integer indicates the number of characters
to compare. The last option of "true"
ignores case.

Contains Methods - Tests if a substring is contained with the string instance under
various conditions, and returns either “True” or “False”.

Method Example Description
Contains [text1].Contains([text2]) Returns "True" if the specified substring
occurs within the string instance.
EndsWith [text1].EndsWith([text2]) Returns "True" if the end of the string
instance matches the specified string.
StartsWith [text1].StartsWith([text2]) Returns "True" if the start of the string
instance matches the specified string.

Modify Methods – The first two methods specify a substring within a string instance
and returns a string with the substring deleted (Remove), or a string with all characters deleted
except for the substring (SubString). Insert returns a string in which the specified string is
inserted at a specified position.

Method Example Description
Remove [text1].Remove(3,5) Returns a string in which a specified
number of characters in the current
instance beginning at a specified position
have been deleted. If the second number
isn't specified, characters will be deleted
up to the end of the string.
SubString [text1].SubString(3,5) Returns a substring from the string
instance. The substring starts at a
specified character position and has a
specified length. If length is omitted, the
substring continues to the end of the
string.

Insert [text1].Insert(5,[text2] Returns a string in which the specified
string is inserted at a specified position in
the string instance.

Format Methods – Converts a string to another format, such as uppercase or
lowercase. The Format method can replace specified items within a string or paragraph with
numerical or text data.

Method Example Description
ToUpper [text1].ToUpper() Returns a copy of the string converted to

uppercase.

ToLower [text1].ToLower() Returns a copy of the string converted to

lowercase.

Format Format("The outside
temperature is {0:N1} F or
{1:N2} C",[num1],[num2])

Replaces the formatted items in a string
with the string representations of the
listed objects. In this example the output
would be:"The outside temperature is
47.3 F or 8.52 C"

ToCharArray [text1].ToCharArray(3.5) Returns an array of characters from the
specified instance. Optional parameters
indicate starting position and length.

(Note: this method only works when
nested within other methods, such as
“Trim” or “IndexOfAny”.)

Trim Methods – Returns a string with the specified characters trimmed off the
beginning, end, or both.

Method Example Description

Trim [text1].Trim() Removes all leading and trailing white-
space characters from the string instance.

Trim [text1].Trim([text2].
ToCharArray())

Removes all leading and trailing
occurrences of a set of characters
specified in an array from the string
instance.

TrimStart [text1].TrimStart([text2].
ToCharArray())

Removes all leading occurrences of a set
of characters specified in an array from
the string instance.

TrimEnd [text1].TrimEnd([text2].
ToCharArray())

Removes all trailing occurrences of a set
of characters specified in an array from
the string instance.

Index Methods – Returns the position of a string or character in a string or substring
depending on specified criteria. The IndexOfAny method will return the first position of any
character in a specified character array in a string or substring.

Method Example Description
IndexOf [text1].IndexOf("-") Returns the position of the first
occurrence of the specified character in
the string instance.

IndexOf [text1].IndexOf("-",5,8) Returns the position of the specified
character in the string instance. The
search starts at the specified character
position and continues up to the specified
number of character positions. If this
number isn't specified, the search will
continue to the end of the string.

IndexOf [text1].IndexOf([text2]) Returns the position of the first
occurrence of the specified string in the
string instance

IndexOf [text1].IndexOf([text2],5,8) Returns the position of the specified string
in the string instance. The search starts at
the specified character position and
continues up to the specified number of
character positions. If this number isn't
specified, the search will continue to the
end of the string.

LastIndexOf [text1].LastIndexOf("-") Returns the position of the last occurrence
of the specified character in the string
instance..

LastIndexOf [text1].LastIndexOf("-",5,8) Returns the position of the specified
character in the string instance. The
search starts at the specified character
position and continues backwards up to
the specified number of character
positions. If this number isn't specified,
the search will continue to the beginning
of the string.

LastIndexOf [text1].LastIndexOf([text2]) Returns the index position of the last
occurrence of a specified string within this
instance.

LastIndexOf [text1].LastIndexOf([text2],5,8) Returns the index position of the specified
string in the string instance. The search
starts at the specified character position
and proceeds backward up to the
specified number of character positions. If
this number isn't specified, the search
continues to the beginning of the string.

IndexOfAny [text1].IndexOfAny([text2].

ToCharArray())

Returns the position of the first
occurrence in the instance of any
character in a specified array.

IndexOfAny [text1].IndexOfAny([text2].
ToCharArray(),1,5)

Returns the position of the first
occurrence in the instance of any
character in a specified array. The search
starts at a specified character position and
examines a specified number of character
positions. If this number isn't specified,

the search continues to the end of the
string.

#Formulas: Numeric Operators and Methods

The 40 numeric operators and methods listed here provide a numeric output based on numeric
inputs. (An input may also include text methods that provide a numeric output, such as the
[text1].Length * 2 +3 formula mentioned previously.)
Several numeric operators and methods can be combined into one complex formula you’re
looking for a certain kind of output. An example is:
Sqrt(Pow([num1],2)+Pow([num2],2))
This formula calculates the length of the hypotenuse of a right triangle.

When using two or more operator types in one formula, the order of precedence for the
calculation is as follows:
1) Unary (such as –[num1])
2) Multiplicative
3) Additive
4) Relational
If parentheses are used, like those in methods like Max(), Min(), Truncate(), etc., the
expressions within the parentheses are evaluated first.

Additive Operators - Basic addition and subtraction formulas.

Formula Example Description
+ [num1]+[num2] Returns the sum of two or more numbers
-

[num1]-[num2] Returns one or more numbers subtracted

from another.

Multiplicative Operators - Basic multiplication and division formulas.

Formula Example Description
% [num1]%[num2] Returns the remainder of dividing the
specified numbers (must be integers and
(num2 != 0)

* [num1]*[num2] Returns the result of multiplying two or

more numbers.

/ [num1]/[num2] Returns the result of dividing two numbers

(num2 != 0)

Sign Formulas - These formulas handle the sign (positive or negative) of a number.

Formula Example Description
Abs Abs([num1]) Returns the absolute value of the given

number

Sign Sign([num1]) Either 1 or -1 is returned, indicating the sign

of the given number.

-

-[num1] Returns the negation of the given number.

Calculation Formulas - Basic logarithmic and exponential functions.

Formula Example Description
Sqrt Sqrt([num1]) Calculates the square root of the specified

number (num1>=0).

Pow Pow([num1],[num2]) Returns the first number raised to a power
specified by the second number.
Exp Exp([num1]) Returns the natural logarithm, ꬲ, raised to

the specified power.

Log Log([num1]) Returns the natural logarithm of a specified

number (base ꬲ).

Log10 Log10([num1]) Returns the logarithm of a specified number

(base 10).

Log(number,base) Log([num1],[num2]) Returns the logarithm of a specified number

(base specified in formula)..

Compare Formulas - Returns the larger or smaller of two numbers.

Formula Example Description
Max Max([num1],[num2]) Returns the larger of the two specified

numbers

Min Min([num1],[num2]) Returns the smaller of the two specified

numbers

Constant Formulas - Constants that can be used in formulas are PI (π) and the natural
logarithmic base (ꬲ).

Formula Example Description
PI PI * Pow([num1],2) This is the constant Pi, π ,which is ratio of
the circumference of a circle to its
diameter.

E Pow(E, [num1]) This is the constant, ꬲ, which is the natural

logarithmic base.

Relational Operators - Compares two number for greater than, less than, or equal to.
Formula Example Description
> If([num1]>[num2],[num1],[num2]) The "greater than" operator only works in a

conditional test.

< If([num1]<[num2],[num1],[num2]) The "less than" operator only works in a

conditional test.

>= If([num1]>=[num2],[num1],[num2]) The "greater than or equal to" operator
only works in a conditional test
<= If([num1]<=[num2],[num1],[num2]) The "less than or equal to" operator only

works in a conditional test.

= If([num1]=[num2],[num1],[num2]) The "equality" operator only works in a

conditional test.

Rounding and Truncating Formulas – Rounds or truncates a decimal number.
Formula Example Description
Truncate Truncate([num1]) Calculates the integer part of a specified

decimal number.

Ceiling Ceiling([num1]) Returns the smallest integer that is greater
than or equal to the specified decimal
number.

Floor Floor([num1]) Returns the largest integer less than or
equal to the specified decimal number.
Round Round([num1]) Rounds the given value to the nearest
integer. If the value if it is midway between
two integers, the nearest even integer is
returned.

Round(number,
precision)

Round([num1],3) Rounds the given value to a specified
number of fractional digits.

Trigonometric Formulas – These formulas include angle as the input or output.
Formula Example Description
Tan Tan([num1]) Returns the tangent of the specified angle.
Atan2 Atan2([num1],[num2]) Returns the angle whose tangent is the
quotient of the two numbers (num_2 != 0).
Cos Cos([num1]) Returns the cosine of the specified angle
Acos Acos([num1]) Returns the angle whose cosine is the
specified number (Abs(num_1) <= 1).

Sin Sin([num1]) Returns the sine of the specified angle.
Asin Asin([num1]) Returns the angle whose sine is the
specified number (Abs(num_1) <= 1)
Cosh Cosh([num1]) Returns the hyperbolic cosine of the

specified angle.

Sinh Sinh([num1]) Returns the hyperbolic sine of the specified

angle.

Tanh Tanh([num1]) Returns the hyperbolic tangent of the

specified angle.

# Formulas: Currency Operators and Methods

This formula type is used exclusively for financial calculations. The data type is based on
currency, but numerical data can be used in the calculation for multiplication, etc. It’s possible
to use text methods that provide a numeric output, but not recommended.
Currency formulas use the same operators and methods as the Numeric formulas, so they
won’t be listed again here. Any of the methods and operators in the: Additive, Multiplicative,
Compare, Relational, Rounding and Truncating, and Sign categories can be used in currency formulas.
Any of the formulas in the Calculation, Constant, Trigonometric categories should not be used for
currency calculations.
An example formula is:
Min([price1]+[price1]*[tax]+[shipping1]+[fee1],[price2]+[price2]*[tax]+[shipping2]+[fee2])
This formula determines the lower price for two different purchase options.
When using two or more operator types in one formula, the order of precedence for the
calculation is as follows:
1) Unary (such as –[num1])
2) Multiplicative
3) Additive
4) Relational

If parentheses are used, like those in methods like Max(), Min(), Truncate(), etc., the
expressions within the parentheses are evaluated first.

# Formulas: Date Methods

Only three formulas currently exist for the Date Field Types. The TimeSpan formula determines the
time between two dates, and the AddTime formula calculates the date offset from a given
date. The numeric output for TimeSpan can be used as a numeric input for other types of
formulas. The numeric output of other types of formulas can be use as the “int amount” input
for the AddTime formula. The Today() formula has no argument and returns today’s date as the
output, which can be used as an input for other formulas that have a date value as an
argument.

Formula Example Description
TimeSpan TimeSpan([d1],[d2],“days”) Calculates the time period (double) between
two dates in “days”, “months”, or “years”. d1
and d2 have the “Date” Field Type. The output
in the example is in “months”. The Field Type
must be set as Formula–Numeric.

AddTime AddTime([d1],2,”months”) Returns a date after adding an offset amount to
the given date where the offset is an integer in
“days”, “months”, or “years”. The offset in the
example is in “days”. The Field Type must be set
as Formula–Date.

Today() TimeSpan([d1],Today(), “days”) Calculates the number of days since d1.

# Formulas: If – Then – Else Function

The If - Then - Else function is another special case that can be used for numeric, text, and
currency formulas. The If - Then - Else clauses should all be text-based for text formulas, based
on numbers for numeric formulas, and based on currency for currency formulas. In some cases,
a numeric output is accepted for text-based If -Then - Else formulas, and vice-versa.
The following table shows examples of the If -Then -Else formula based on numbers and based
on text:

Formula Example Description
If If([num1]>[num2],[num1],[num2]) This is an If-Then-Else test for greater
than. Also works for less than (<), less
than or equal to (<=), greater than or
equal to (>=), or equals (=). This works for
both text and numeric formula types.
Example returns the max of the two
numbers.

If If([text1].Contains([text2]),[text1],[text2]) This If-Then-Else test only works as a text
formula. The “If” clause must be a text
method with a true or false output like
Equals, StartsWith, etc. Example returns
text1 if text1 contains text2. Otherwise,
text2 is returned.

If -Then -Else statements can also be nested as shown in the following example.
If([num1]>[num2], If([text1].Contains([text2]),[text1],[text2]), [text1])
Note that this will only work as a text formula. If you change the outputs to numbers as in the following
example:
If([num1]>[num2],If([text1].Contains([text2]),[num1],[num2]),[num1])
The formula will work both as a text, numeric, and currency formula. All outputs must either be text,
numeric, or currency for the formula to work.

# Formulas: Format Method

The Format method is a special kind of text formula that can be used to replace all { } items
within a string or paragraph with corresponding data listed at the end, which can be numerical,
or text, or date data.
The formula starts with the string or paragraph followed by one or more objects or expressions
that will be converted to strings and inserted at a specified place in the format string. For
example:
Format("The high temperature on {0:d} was {1:n1} 0F or {2:n2} 0C",[date],[num1],[num2])
replaces the formatted items in a string with the string representations of the listed objects. In
this example, the output would be: "The high temperature on 3/28/2020 was 47.3 0F or 8.52
0C".
The {0:d} item above applies the "d" format (date) to the first object in list. The {1:n1} item
refers to a number with one digit after the decimal.

Each formatted item must have the opening and closing braces. A format item has this syntax:
{index[,alignment][:formatString]}
where the brackets indicate optional parameters.
index (required) - The zero-based index of the argument whose string representation is to be
included at this position in the string.
alignment (optional) - A signed integer that indicates the total length of the field into which the
argument is inserted and whether it is right-aligned (a positive integer) or left-aligned (a
negative integer). If not specified, the argument is inserted at the corresponding position with
no leading or trailing spaces.
formatString (optional) - A string that specifies the format of the corresponding argument's
result string. This can be one of the following letters: t (time), d (date), n (number), c
(currency), and p (percentage). Text values don't need this specifier. If omitted, a ToString
method will be used to produce its string representation. An optional integer after the letter
indicates decimal precision.

# Null Test for Data Types

If one of the data types (Text, Numeric, Currency, Date, or DateTime) hasn’t been assigned a
value, it is considered to be null. The only exception is in the Text data type, where you can
assign a value of “null” (string Text = null), which is different from an empty string with no
assigned value.
Note: the following tests are usually used as the test argument in an If -Then -Else function described
in the previous section. When used by itself, the test must be set to the appropriate formula
type and will return either “true or “false”.

Null Test for Text –These formulas test a string of text for the specified condition.
Returns either “True” or “False”.

Method Example Description
Test for null [text1]=null Returns true if the string is a "null" string
Test for empty [text1].Equals("") Returns true if the string is empty (no

assigned value)

In this application, we consider a Text data type to be null if it is in any of these three states: it
has a value of “null”, is empty (no assigned value), or consists exclusively of white-space characters.
Therefore, we’ll be using the following formula as the Null Test for Text:
Test for null, empty,
or white-space

IsNullOrWhiteSpace([text1]) Returns true if the string is either null,

empty, or consists exclusively of white-
space characters.

Null Test for Numeric Values
If a numeric value has been declared, but hasn’t been assigned a value, it will be automatically
assigned a default value of 0. But in certain cases where a null value is possible, the same
method that was used for text should be used (IsNullOrWhiteSpace) to test for null. This

formula will first convert the numeric value to a string ([num1].ToString()), and then use the null
test method: (IsNullOrWhiteSpace):

Method Example Description
Test for null IsNullOrWhiteSpace([num1].ToString()) Returns true if the numeric value hasn’t

been assigned a value.

If a number has a value of null, and is used in a formula, it will generate an error. The following
formula will convert a null value to zero, so it can be used in the formula. If the number isn’t
null, the same number is returned:
If(IsNullOrWhiteSpace([num1].ToString()),0,num1)

Null Test for Currency Values
If a currency value has been declared, but hasn’t been assigned a value, it will be automatically
assigned a default value of 0. But in certain cases where a null value is possible, the same
method that was used for numeric values should be used.
Method Example Description
Test for null IsNullOrWhiteSpace([text1].ToString()) Returns true if the currency value hasn’t

been assigned a value.

If a currency value has a value of null, and is used in a formula, it will generate an error. The
following formula will convert a null value to zero, so it can be used in the formula. If the
currency value isn’t null, the same value is returned:
If(IsNullOrWhiteSpace([amount1].ToString()),0,amount1)

Null Test for Dates – If a Field Type set to “Date” isn’t set to a value, it will be stored
as a null date in the database as 00-00-0001. Therefore, if the date string contains “001”, it is
considered null.
Method Example Description
If If([date_of_response]].ToString().
Contains("001"), "Closed","Open")

Returns “Closed” if the given date is null.
Otherwise “Open” is returned. Must be set as
Formula–Text.

If a date has a value of null, and is used in a date method, as described here, it will generate an
error.

Null Test for Documents – If a Field Type is set to “File Attachment”, this formula
can be used to determine if a file is attached or not:
Method Example Description
If if(IsNullOrWhiteSpace([Doc1]),
"Empty","Uploaded")

Returns “Empty” if a file hasn’t been uploaded
yet for Doc1. Otherwise “Uploaded” is
returned. Must be set as Formula–Text.

Note that there are no formulas for documents other than a null test.

