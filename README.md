# Safe Workplace Contact Tracing App – Power Platform Solution

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
- Use the Model Driven App to report Employee and Visitor health status and presence Human Resource Admin)

## Deploying Safe Workplace Contact Tracing App

This document provides step by step instructions to setup the Safe Workplace App.

### Step 1. Download the Deployment Package

Download the latest deployment package (.zip)

[![Download Contact Tracing Solution](https://raw.githubusercontent.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/master/assets/icons/DownloadButton.svg)](https://github.com//AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/releases/latest/download/ContactTracing.zip)

Before extracting the .zip file, ensure that you unblock it.

1. > Right click the .zip file, select **Properties**

2. > In the properties dialog box, select Unblock, then select Apply followed by **OK**.

On extracting the .zip file, you will see the following in the extracted
folder:

| Folder  | Description                                                                                                                |
| ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Package | Contains the Package Developer tool and the package that you will deploy later to set up the solution in your environment.  For more information see Option C: Install the app from the deployment package |

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

### Step 3. Install the App

Follow the steps before to install Safe Workplace Tracing App along with
configuration

You can install the app by downloading it here: [![Download Contact Tracing Solution](https://raw.githubusercontent.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/master/assets/icons/DownloadButton.svg)](https://github.com//AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/releases/latest/download/ContactTracing.zip)

*Install the app from the deployment package*

1. Navigate to the location where you extracted the deployment package (.zip), you will find a Package folder.

2. Go to <https://make.powerapps.com> and login, if needed, with your admin credentials to the environment

    ![IMG2](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2002.png)

3. Click on the settings Icon and then select then select **continue**  

4. The Settings area for Dynamics 365 opens. Click on the settings option on the menu!

    ![IMG3](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2003.png)

5. Click on the Solutions option under the Customization menu. This will open the Solutions page.

6. Click on the Import Button

    ![IMG4](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2004.png)

7. The Import solution form opens. Select the solution package to import by clicking on the choose File button, select the package previously downloaded and click OPEN. The Form should look as follows:

    ![IMG5](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2005.png)

8.  Select **Next**

9.  The import tool will gather the solution information. Will display the Name, Publisher, and Package type. The following information should be displayed:

    ![IMG6](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2006.png)

10. Select **Next**

11. An Import Options screen will be displayed. Click on the Import Button on this form. The import process starts running, the screen will look as follows:

    ![IMG7](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2007.png)

12. Once the import process bar shows as completed, the importing solution form will indicate if the import was successfully completed. There might be some warnings displayed, but as long as there are no issues listed, the import has been completed.

13. Click on the Close button to close the import page

14. The "ContactTracing" solution now should be listed in the ALL SOLUTIONS view, as follows:

    ![IMG8](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2008.png)

15. Close the browser session for the Dynamics 365 settings and navigate to Power Apps and select your environment. Click on the Apps Button. The Safe Workplace App should be now listed

    ![IMG9](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2009.png)

Installation will add the configuration for the Safe Workplace Contact Tracing app

Select the Admin App to open the model driven app that lets you configure the rest of the deployment settings.  The admin app has several entities where you can add and manage data for your system.  You can use the area picker in the lower part of the left navigation pane to select a different area (Safe Place or Administration).

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

For Employee Users to use the canvas app on their mobile devices, the app must be shared with them.  It is easier to use Azure AD groups to easily share apps with groups of users.

It is important to note that you must make sure the user and/or group already has access to the environment. Typically, you would have already added users or groups while setting up your environment. You can also follow the steps below to add users to your environment and provide the correct access before sharing.

1. Sign into [Power Apps](https://make.powerapps.com/)

2. Select **Apps** to view list of Apps

3. Select the mobile app then select **Share**

    ![IMG14](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2014.png)

4. Specify the Azure AD group or users that the app will be shared with to add user

    ![IMG15](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2015.png)

5. Next, permission to the entities will need to be provided. To assign the respective user role necessary, the Common Data Service User role should be selected first. Once Common Data User role is selected, you can then assign the applicable role for the user, Safe Workplace Super User, Safe Workplace Coordinator, or Safe Workplace Employee)

    ![IMG16](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2016.png)

    ![IMG17](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2017.png)

    ![IMG18](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2018.png)

### Step 7: Pin Mobile app to Home screen on your phone (optional)

As an option you can pin your mobile app to your home screen, to avoid the need to open the Power Apps application to then access the Safe Workplace App. To do so, follow these steps

1. Open your Power Apps application on your mobile Device

2. The Safe Workplace App should be listed, Click on the **"…"** Icon. The following options should be displayed at the bottom: Details, Open, Pin to Home, Favorite

    ![IMG19](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2019.png)

3. Click on the **Pin to Home Option**

    ![IMG20](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2020.png)

4. There, click on the Icon indicated here to add the app to the home screen

    ![IMG21](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2021.png)

5. Click on the **“add to home screen option”** as show on the image above

    ![IMG22](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2022.png)

6. Click on the **“add”** option. Once completed, the app is going to be shown as any other home screen of your mobile device

    ![IMG23](https://github.com/AKA-Enterprise-Solutions/SafeWorkplace-ContactTracing/blob/master/assets/screenshots/Safe%20Workplace%20IMG%2023.png)

### Step 8: Share Model Driven App with Organization Admins

Model Driven App must be shared with Organization Admins for use. To do so, be sure the user and/or group to which the app is being shared with already has access to the environment.

1. Sign into [Power Apps](https://make.powerapps.com/)

2. Select **Apps** to view a full list of Apps

3. Select **Model Driven App** and select **Share**

4. Specify the Azure AD group or admin users that the app will be shared with.  Assign Safe Workplace Super User (Admin) security role and share
