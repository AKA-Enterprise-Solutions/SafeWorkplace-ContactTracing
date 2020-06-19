# Safe Workplace Contact Tracing App – Power Platform Solution

[![GitHub Release Date](https://img.shields.io/github/release-date/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing?label=Released&style=for-the-badge)](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/releases)
[![GitHub labels](https://img.shields.io/github/labels/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/bug?label=Report%20Issues&style=for-the-badge)](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/issues/new?assignees=Adramca&labels=bug%2C+under+review&template=bug_report.md)
[![Twitter Follow](https://img.shields.io/twitter/follow/akaesny?color=blue&label=Click%20Here%20Follow%20us&style=for-the-badge)](https://twitter.com/akaesny)
===
[![GitHub All Releases](https://img.shields.io/github/downloads/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/total?color=green&style=for-the-badge&label=💻1.Download%20Core%20Package)](https://github.com//AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/releases/latest/download/ContactTracing_Core_Managed.zip)

[![GitHub All Releases](https://img.shields.io/github/downloads/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/total?color=green&style=for-the-badge&label=📲2.Download%20Mobile%20Package)](https://github.com//AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/releases/latest/download/SafeWorkplace_CanvasApp.zip)

## Overview

In response to COVID-19, the Safe Workplace Contact Tracing application is a solution set to provide SMB organizations the ability to track the location for both employees and visitors while they are physically on company premises. As this information is collected, when required Human Resource departments will be able to provide accurate tracing of all
locations visited by an employee or a visitor due to COVID-19 concerns.  

The Safe Workplace Contact Tracing App features include the following:

- Ability to configure location zones, so employees can easily identify areas where they will be able to report their location
- Provide employees with the ability to easily report their whereabouts, selecting the zone where they are at any point in time,as well as their movements across different zones on company premises
- Provide functionality for HR resources to track visitors’ locations while on premises, and to capture basic information about them and their health for reporting purposes  
- Ability for employees or HR users assisting visitors entering company premises, to complete required survey certifying overall health
- Provide the HR department with the functionality needed to be able to effectively inquire and report an employee’s whereabouts,interactions and location/contact tracing data
  
## Navigating the App

- Download and deploy the Safe Workplace Model Driven App (Admin)
- Download and deploy the Safe Workplace CanvasApp (Employee)
- Use the Model Driven App to manage master data and dashboards (Human Resource Admin)
- Use the mobile CanvasApp to track Employee location and presence (Business Admin)
- Use the mobile CanvasApp to record Employee health (Business Admin/Employee)
- Use the Model Driven App to report Employee and Visitor health status and presence (Human Resource Admin)
- Use the Model Driven App to create visitor's contact information, health information, report health updates and presence (Human Resource desiginated Coordinators)

## Demo Video

### Canvas App (Mobile) Demo

Click 👇 to see the demo video (ctrl + click to open in Vimeo)

[![Canvas Apps Demo](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/VideoImage.png)](https://vimeo.com/430412668)

#### Model-driven App Demo

> Coming soon!!

## Deploying Safe Workplace Contact Tracing App

This document provides step by step instructions to setup the Safe Workplace App.

### Step 1. Download the Deployment Packages

Download the latest deployment packages

1. Core (Model-driven App) Package 👉 [![Download Contact Tracing Solution](https://raw.githubusercontent.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/master/assets/icons/DownloadButton.svg)](https://github.com//AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/releases/latest/download/ContactTracing.zip)

2. Canvas App Package 👉 [![Download Contact Tracing Solution](https://raw.githubusercontent.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/master/assets/icons/DownloadButton.svg)](https://github.com//AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/releases/latest/download/ContactTracing.zip)

### Step 2. Sign Up for Power Apps and Create an Environment

If you do not already have Power Apps, sign up for Power Apps and
purchase an appropriate license.  Additional information regarding
purchasing Power Apps and Licensing can be access here:

- [Power Apps Pricing](https://powerapps.microsoft.com/pricing/)

- [Purchase Power Apps](https://docs.microsoft.com/power-platform/admin/signup-for-powerapps-admin)

Once you have purchased Power Apps, create an environment with a Common
Data Service database.

1. Sign into [Power Platform Admin Center](https://aka.ms/ppac)

2. Create a Common Data Service environment with the database. For  more information, see [Create and Manage Environments](https://docs.microsoft.com/en-us/power-platform/admin/create-environment)

    > [NOTE] While creating the database, if you select a security group for the database, the apps can be shared only with users that are members of the security group.

3. Create appropriate users in your environment. For more information, see [Create Users and Assign Security Roles](https://docs.microsoft.com/en-us/power-platform/admin/create-users-assign-online-security-roles)

    ![IMG1](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2001.png)

### Step 3. Install the Apps

Follow the steps before to install Safe Workplace Tracing App along with configuration

*Install the app using the deployment packages*

1. Navigate to the location where you downloaded the deployment packages.

2. Go to <https://make.powerapps.com> and login, if needed, with your admin credentials to the environment

    ![IMG2](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2002.png)

3. Click on **Solutions** from the left navigation

    ![IMG3](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2003.png)

4. Click on **Import** from top ribbon. This will open a pop-up window to select **Solution Package**

    ![IMG4](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2004.png)

5. Select *Choose file* and navigate to the location of package named "**ContactTracing_Core_Managed.zip**"

6. Ensure the solution name is correct and select **Next**

    ![IMG5](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2005.png)

7. On the next window, select the "*Enable any SDK message…*" checkbox.  Once checkbox is checked, click on **Import**

    ![IMG6](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2006.png)

8. The import process starts running

9. *(optional)* After import is complete, select *Download Log File* and save it. This is just for future reference should any issues arise. Finally, select **Close**

    ![IMG7](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2007.png)

10. Now, you should see "Safe Workplace – Contact Tracing" in the list of installed solutions

    ![IMG8](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2008.png)

11. Click on **Apps** in the left navigation pane to access the apps installed. The Safe Workplace Admin app should be now listed

12. Click on Import Canvas App on the Top menu

    ![Step12](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Step12.png)

13. Choose the package file to import form is now open. Make sure you select the "**SafeWorkplace_CanvasApp.zip**" file from the location where you downloaded the packages

    ![Step13](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Step13.png)

14. Once the upload is completed, the following validation page is displayed

    ![Step14](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Step14.png)

15. Click on the action icon next to the item marked with a *Red Exclamation Icon* to setup the common data service connection for the Canvas App. Once the icon is clicked, the *Import Setup* form is displayed

    ![Step15](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Step15.png)

16. Click on the "**Create New**" button. This will open a new browser window. Click on the "**Create a Connection button**" there. This will open the new connection form to choose a Connection for creation

    ![Step16](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Step16.png)

17. Select the Common Data Service option. Click on the "+" icon on the right. On the confirmation message to request creation, click on the "*CREATE*" button. The following message is displayed

    ![Step17](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Step17.png)

18. The application might ask you to login to your environment. Once the process is completed, the data connection is added

    ![Step18](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Step18.png)

19. Go back to the import setup. The newly created connection should be there. Select it and then click on **SAVE**

    ![Step19](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Step19.png)

20. The Related resource for data connection is now resolved, the import button should be enabled now. Click on **IMPORT**

21. Once the import is completed, the following message should be displayed

    ![Step21](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Step21.png)

22. Click on the Apps button again. Now the Safe Workplace Canvas App should be displayed.

    ![IMG9](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2009.png)

Installation will add the configuration for the Safe Workplace Contact Tracing app

Select the Admin App to open the model driven app that lets you configure the rest of the deployment settings.  The admin app has several entities where you can add and manage data for your system.  You can use the area picker in the lower part of the left navigation pane to select a different area (Safe Place or Administration). Please review the demo of the solution to obtain more infromation about how to use the Administration options of the app.

![IMG10](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2010.png)

### Step 4: Update the app branding and tracking level

You can change the app icon or display name of the Admin and mobile apps
to match the branding of your organization.  

1. Select the Safe Workplace Admin App on the list of apps. Click on the Settings option on the main navigation menu on the top left navigation

    ![IMG11](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2011.png)

2. The App settings form will open on the right side of the screen.

3. Click on the **Edit App Name** link. This will open the app designer form

    ![IMG12](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2012.png)

4. Click on the Properties Tab of the App details section. The following elements can be changed:
    1. To select a custom image for the app icon as per your organization branding, uncheck the use default image checkbox and then select the icon file of your choice

    2. If necessary, update the Description or Display Name of the app

    3. Select **Save and Close and then Publish**

    ![IMG13](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2013.png)

To update the App Name and sharing settings for the mobile app, follow these steps

1. Select the Safe Workplace App on the list of apps. Click on the Settings option on the main navigation menu on the top left navigation

2. The App settings form will open on the right side of the screen.

3. Click on the **Edit App Name** link and then enter the new App Name.

4. Select **Yes or No** in the Pass Assignment option to allow the app to be shared with users without a Per user Plan

5. Select **Save** in the lower-right corner to save changes

### Step 5: Add Azure Application Insights key to mobile apps for telemetry (optional)

Optionally, you can use Azure Application Insights to collect detailed telemetry for your mobile apps (canvas apps) to get insights on the app usage. For additional information on this, see [Analyze app telemetry using Application Insights](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/application-insights).

### Step 6: Share Canvas App with users in the organization

For Employees to use the canvas app on their mobile devices, the app must be shared with them.  It is easier to use Azure AD groups to easily share apps with groups of users.

It is important to note that you must make sure the user and/or group already has access to the environment. Typically, you would have already added users or groups while setting up your environment. You can also follow the steps below to add users to your environment and provide the correct access before sharing. For more information on how to create users and assign security see [Create Users and Assign Security Roles](https://docs.microsoft.com/en-us/power-platform/admin/create-users-assign-online-security-roles)

1. Sign into [Power Apps](https://make.powerapps.com/)

2. Select **Apps** to view list of Apps

3. Select the mobile app then select **Share**

    ![IMG14](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2014.png)

4. Specify the Azure AD group or users that the app will be shared with to add user

    ![IMG15](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2015.JPG)

5. Next, permission to the entities will need to be provided. To assign the respective user role necessary, the Common Data Service User role should be selected first. Once Common Data User role is selected, you can then assign the applicable role for the user, Safe Workplace Super User, Safe Workplace Coordinator, or Safe Workplace Employee)

    ![IMG16](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2016.png)

    ![IMG17](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2017.png)

    ![IMG18](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2018.png)

### Step 7: Pin Mobile app to Home screen on your phone (optional)

As an option you can pin your mobile app to your home screen, to avoid the need to open the Power Apps application to then access the Safe Workplace App. To do so, follow these steps

1. Open your Power Apps application on your mobile Device

2. The Safe Workplace App should be listed, Click on the **"…"** Icon. The following options should be displayed at the bottom: Details, Open, Pin to Home, Favorite

    ![IMG19](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2019.jpg)

3. Click on the **Pin to Home Option**

    ![IMG20](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2020.jpg)

4. There, click on the Icon indicated here to add the app to the home screen

    ![IMG21](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2021.jpg)

5. Click on the **“add to home screen option”** as show on the image above

    ![IMG22](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2022.jpg)

6. Click on the **“add”** option. Once completed, the app is going to be shown as any other home screen of your mobile device

    ![IMG23](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2023.jpg)

### Step 8: Share Model Driven App with Organization Admins

Model Driven App must be shared with Organization Admins for use. To do so, be sure the user and/or group to which the app is being shared with already has access to the environment.

1. Sign into [Power Apps](https://make.powerapps.com/)

2. Select **Apps** to view a full list of Apps

3. Select **Model Driven App** and select **Share**

4. Specify the Azure AD group or admin users that the app will be shared with.  Assign Safe Workplace Super User (Admin) security role and share

### Step 9: Set Flows Connections and Enable them for Execution

You must set the connections and enable the following flows that help in various processess in the solution. The following flows will need to go through the steps indicated below:
  
- CDS: Flow > Automated Presence Checkout
- CDS: Flow > Health Notification to HR
- CDS: Flow > Set Preferred location in Contact

Follow these steps:

1. Sign into [Power Auotmate](https://flow.microsoft.com/)

2. In the left pane select **Solutions**. From the solution list, select **Safe Workplace Contact Tracing** to open solution.

   ![IMG24](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2024.png)

3. In the solution, filter on **Flow** to find all the flows.

   ![IMG25](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2025.png)

4. Select the flow name to open the flow definition. For example, **CDS: Flow > Automated Presence Checkout**

5. Double click on the flow name to open it. It will take you to the details form.  It should look like this

   ![IMG26](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2026.png)

6. Click on the **Edit** button on the Menu.  A screen confriming the connections for the flow will be displayed. It will look like this:

   ![IMG27](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2027.png)

7. Click on **Continue** to update all your connections and then click on **Save** to save the changes to the flow.  Then click on the **Back** arrow to go back to the flow details page

   ![IMG28](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2028.png)

8. Select **Turn On** and then close the browser session for the flow being edited. Flow is now active.

9. Perform steps 4-8 for each of the flows listed above

### Issues and Feedback

To report any issues or provide feedback regarding the Safe Workplace Contact Tracing App, [click here](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/issues/new?assignees=Adramca&labels=bug%2C+under+review&template=bug_report.md)
