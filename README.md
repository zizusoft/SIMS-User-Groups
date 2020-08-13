# Creating a SIMS User Account

In order for any application to access data from SIMS through the Buisness Objects, the application must be provided with a SIMS username and password.

Users in SIMS can be granted different levels of access depending on the depth of data the user / application needs access to.

For the application you are about to install, a SIMS user group is provided which can be imported into SIMS - this user group has the minimum permissions asociated with it that are needed to run the application.

***There is no requirement to carry out the below steps to create a new SIMS user to use the application you are about to intall. You can use an existing SIMS user as long as they have suitable permissions.***

To create a new user and import group permission, you will need to log into SIMS with an administrator user that has permission to create users, import user groups and modify permissions. The default administrator in SIMS is called **sysman**. If you are not sure how to create new users - speak to your Network Manager.

## Downloading the SIMS User Group

Navigate to the **Releases** section of this repository and select the zip file that corresponds to your SIMS Client Version.

Your SIMS client version can be found on the splash screen when you log into SIMS:

![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/05/01-00-28-41-sims-VersionNumber.PNG)

Extract the .zip file and you will find a set of .xml files, each named as one of the apps that ZizuSoft Ltd. offers. Find the .xml file that relates to the app you want to install, and delete the others.

***Note: In the below guide, we will assume you are adding a SIMS user to use the Cover Diary App, however the process is similar for other apps too***

## Importing a SIMS User Group

1. In SIMS navigate to **Focus > System Manager > Import Groups**
  
  ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/04/30-23-23-03-sims-ImportGroup.png)
  
2. Click the **Select Import File** button:
  
  ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/04/30-23-25-42-sims-SelectImport.fw.png)
  
3. Navigate to the .xml file downloaded (as instructed earlier).
  
4. The User Group for the application should be displayed. Click the **Import** button to import the group to SIMS.
  
  ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/05/01-00-25-15-sims-ImportGroup2.PNG)
  

## Creating a New SIMS User

1. Navigate to **Focus > System Manager > Manage Users**
  
  ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/05/01-00-34-12-sims-UserManager.png)
  
2. Press the **New** button:
  
  ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/05/01-11-44-42-sims-NewUser.PNG)
  
3. Give your new user a surname and forename such as **coverdiary** for both. There is no need to complete a date of birth or gender. Click **Continue**.
  
  ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/05/01-11-47-02-SIMS-NewUser2.PNG)
  
4. Next we want to add this user to the permissions group we imported earlier. To do this click the **Add** button on right side of the **Groups** panel.
  
  ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/05/01-11-50-26-sims-AddGroup.PNG)
  
5. Select the imported group from the list and click **OK**
  
  ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/05/01-11-52-36-sims-AddGroup2.PNG)
  
6. At this point, take a look at the **Login Details** panel under section 2. Even though the username text box is greyed out, you can still change the username. It will default to the firstname followed by the lastname. You may wish to edit this something more simple such as just **coverdiary** (rather then coverdiarycoverdiary). You will also need to copy the randomly generated password shown in the texbox below the username:
  
  ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/05/01-11-55-53-sims-LoginDetails.PNG)
  
7. Click **Save**
  
  ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/05/01-11-57-19-sims-UserSave.PNG)
  
8. Close SIMS
  
9. Relaunch SIMS and enter your chosen username (from step 6) and copied password. You should also tick the **Change Password** box:
  
  ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/05/01-12-01-59-sims-ChangePass.PNG)
  
10. Change the password to something more memerable and click **OK**.
  
  *Note: SIMS passwords must be at least 8 characters in length.*
  
  ![](https://raw.githubusercontent.com/zizusoft/Assets/master/2020/05/01-12-03-15-sims-ChangePass2.PNG)
  
11. Close SIMS.
  

You now have a new user with the minimum permissions required to run the application.
