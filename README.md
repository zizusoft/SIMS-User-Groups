# Creating a SIMS User Account

In order for any application to access data from SIMS through the Buisness Objects, the application must be provided with a SIMS username and password.

Users in SIMS can be granted different levels of access depending on the depth of data the user / application needs access to.

For the application you are about to install, a SIMS user group is provided which can be imported into SIMS - this user group has the minimum permissions asociated with it that are needed to run the application.

***There is no requirement to carry out the below steps to create a new SIMS user to use the application you are about to intall. You can use an existing SIMS user you already have set up in your school as long as they have suitable permissions.*** 

***If you want to use a SIMS user that you already have set up in your school, you can check if that user has suitable permissions by clicking the yellow 'Check Permissions' button on the server software's Config.aspx page as shown below.***

<img title="" src="https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-16-41-09-user1.PNG" alt="" width="255">





## Preparing the SIMS User Group

SIMS User Groups are stored as XML files. To find the user group for you application, have a look on the Application Server that the site is running on and look for the **SIMS User Group** folder in the root. In this folder, you should find an .xml file which starts **ZIZU-** as shown below.

<img title="" src="https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-16-46-40-user2.PNG" alt="" width="370">

You will need to update the XML file (open it in Notepad) and modify the **DatabaseVersion** tag on line 4:

<img title="" src="https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-16-50-03-user3.PNG" alt="" width="372">

The DatabaseVersion needs to updated to the DatabaseVersion of SIMS you want to import the permissions for. If you don't update this value to the database value you are using, the import will fail.

Your SIMS database version can be found by logging into SIMS normally and navigating to **Help > About SIMS.NET**.

<img title="" src="https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-16-54-40-user4.PNG" alt="" width="372">

A splash screen will show letting you know the database version number you are using. 

Place this number in the XML file on line 4 in the **DatabaseVersion** tag.





## Importing the SIMS User Group

***Note: In the below guide, we will assume you are adding a SIMS user to use the Cover Diary App, however the process is similar for other apps too***

To create a new user and import group permission, you will need to log into SIMS with an administrator user that has permission to create users, import user groups and modify permissions. The default administrator in SIMS is called **sysman**. If you are not sure how to create new users - speak to your Network Manager.

1. In SIMS navigate to **Focus > System Manager > Import Groups**
   
   <img title="" src="https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-17-07-59-user5.PNG" alt="" width="358">
   

2. Click the **Select Import File** button:
   
   <img title="" src="https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-17-09-29-user6.PNG" alt="" width="362">
   
   

3. Navigate to the .xml file you have prepared (as instructed earlier).
   

4. The User Group for the application should be displayed. Click the **Import** button to import the group to SIMS.
   
   ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-17-10-52-user7.PNG)

## 

## Creating a New SIMS User

1. Navigate to **Focus > System Manager > Manage Users**<img title="" src="https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-19-27-35-user8.PNG" alt="" width="332">
   
   

2. Press the **New** button:
   
   <img title="" src="https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-19-28-11-user9.PNG" alt="" width="276">
   
   

3. Give your new user a surname and forename such as **coverdiary** for both. There is no need to complete a date of birth or gender. Click **Continue**.
   
   ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-19-29-22-user11.PNG)
   

4. Next we want to add this user to the permissions group we imported earlier. To do this click the **Add** button on right side of the **Groups** panel.
   
   ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-19-30-45-user12.PNG)
   

5. Select the imported group from the list and click **OK**
   
   <img title="" src="https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-19-31-41-user13.PNG" alt="" width="281">
   

6. At this point, take a look at the **Login Details** panel under section 2. Even though the username text box is greyed out, you can still change the username. It will default to the firstname followed by the lastname. You may wish to edit this something more simple such as just **coverdiary** (rather then coverdiarycoverdiary). You will also need to copy the randomly generated password shown in the texbox below the username:
   
   ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-19-33-10-user14.PNG)
   

7. Click **Save**
   
   <img title="" src="https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-19-34-12-user16.PNG" alt="" width="342">
   

8. Close SIMS
   

9. Relaunch SIMS and enter your chosen username (from step 6) and copied password. You should also tick the **Change Password** box:
   
   <img title="" src="https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-19-35-23-user17.PNG" alt="" width="220">
   

10. Change the password to something more memerable and click **OK**.
    
    *Note: SIMS passwords must be at least 8 characters in length.*
    
    <img title="" src="https://raw.githubusercontent.com/zizusoft/Assets/master/2021/01/22-19-36-27-user18.PNG" alt="" width="254">
    

11. Close SIMS.
    

You now have a new user with the minimum permissions required to run the application.
