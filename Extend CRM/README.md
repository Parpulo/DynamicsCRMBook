# Extend CRM

What you get from CRM out of the box is limited and therefor the major part of the work done on Dynamics CRM projects is on extensions.
There are 2 common ways to extend CRM:
- Web Resources;
- Plugins

Different developers deal with this differently as there are many options and tool that can help you achieving this.
Personally I prefer to use <a href="https://xrmtoolkit.com/">XRM Toolkit</a> for this purpose, this is not an Open Source Tool but you have a 30-days trail to play around with it.

Here is a Step by Step guide that beginners might find helpful:

1. You want to start by downloading and installing XRM Toolkit, to make sure that installing was done properly open your Visual Studio and you should be able to find this tab added:
![alt tag](https://github.com/Parpulo/DynamicsCRMBook/blob/master/img/xrmtoolkit.PNG)

2. Create a new Class Library Project:
![alt tag](https://github.com/Parpulo/DynamicsCRMBook/blob/master/img/newProject.PNG)

This project will be the place where you will create all the Plugins, the C# code that will extend your Dynamics CRM.

3. Link the Solution that you just created to the CRM instance that you are working:
![alt tag](https://github.com/Parpulo/DynamicsCRMBook/blob/master/img/linkToCMR.PNG)

By clicking this tab a new window will open where you will have to enter the URL of your CRM and your login credentials.

4. Create a new project for your Web Resources:
![alt tag](https://github.com/Parpulo/DynamicsCRMBook/blob/master/img/assets.PNG)

You will be asked to check all the types of files that you want to include such as, html, css, js ect.
Every time you add a new web resource inside the solution you want to update the CRM so the file can be included there too, for this purpose you have to click the file that you mean to add:
![alt tag](https://github.com/Parpulo/DynamicsCRMBook/blob/master/img/addFiles.PNG)

After this you can check your solution inside CRM, under Web Resources click Add Existing and include the file that you just added.
Be aware to keep well organized folders of the Asses Project and create as much global resources as you can, so to reuse them and create standards.

With Plugins is slightly different, you first have to **Register** a plugin, go back to CRM Solution to include this as Existing Plugin.
Every time you update plugins you have to Build and Publish so that changes can affect your CRM.
![alt tag](https://github.com/Parpulo/DynamicsCRMBook/blob/master/img/publish.PNG)
