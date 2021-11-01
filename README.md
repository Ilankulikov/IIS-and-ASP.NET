# Week 3 Project
###### *In this project I have created basic "ASP.NET Core Website".*
###### *For this exersice I used Microsoft Visual Studio and IIS.*

## Web App Installation:

## Step 1:
__Creating new project "ASP.NET Web App" in Microsoft VS__ <br/>
![image](https://user-images.githubusercontent.com/90269123/135636902-114d09a5-3dcc-4cc0-a1f0-0d5c9b5d89f4.png)

__*content of csproj:*__ <br/>
![1](https://user-images.githubusercontent.com/90269123/135638533-dca1a4f3-be00-4bca-a849-6206dd0e6df0.JPG)

## Step 2:
__Importing the 'Newtonsoft.json' library:__ <br/>
__Go to:__ <br/>
__tools -> NuGet Package  Manager -> Manage NuGet Packages for Solution.__ <br/>
![image](https://user-images.githubusercontent.com/90269123/135638217-ac64d441-c2cc-4381-a583-011d6ea9fbde.png)

__*content of csproj after browsing the library:*__ <br/>
![2](https://user-images.githubusercontent.com/90269123/135638678-6891e6a6-40f0-4793-9ad4-39a0bd692f39.JPG)

## Step 3:
__Right click on Solution -> 'Restore NuGet Packages' and right after 'Rebuild Solution'.__ <br/>
__Now We have compiled our project and created the bin and obj folders and binary files.__ <br/>
![image](https://user-images.githubusercontent.com/90269123/135640411-2d8ab759-d964-454f-8d01-4ae10b9f6393.png)

## Step 4:
__Publish your Web App : right click on Web App -> publish .__ <br/>
![image](https://user-images.githubusercontent.com/90269123/135640690-4687ae66-5d99-48a9-9a93-39f8a2ce2be7.png)

__Now folder named "Release" was created in the WebApp/bin folder which contains the necessary files deploy and run our web app.__


__* *In the next steps we will do the deployment of our web app.*__ 

## IIS Configuration and Web App Deployment:

## Step 1:
__Add new Application Pool:__ <br/>
![image](https://user-images.githubusercontent.com/90269123/135642540-6b57fa76-5e43-41d2-a791-b91f9de5c6ad.png)

## Step 2:
__Add new Website and select the Application Pool you have added in Step #1:__ <br/>
![image](https://user-images.githubusercontent.com/90269123/135643047-be98ab46-9062-42b7-adfb-36f09ef17fc5.png)

## Step 3:
__Go to Application Pools , choose the application pool you just created in step #1 and 'Stop' it.__ <br/>
![image](https://user-images.githubusercontent.com/90269123/135643950-41911880-fe7d-4a9c-8d14-734afb12672a.png)


## Step 4:
__Right click on your Website -> Explore , Copy the content of the "Release" folder We have created in Step #4 of 'Web App Installation' to this folder.__

## Step 5:
__Go to Application Pools , choose the application pool you just created in step #1 and 'Start' it.__ <br/>
![image](https://user-images.githubusercontent.com/90269123/135644268-b58d0ac4-0013-4ce9-b290-641001a362a8.png)

###### Congratulations ! Your website are ready, Open your browser and go to http://localhost:80/. 
> *Note: The default port is :80 but you must write the port used in step 2 , in my example it was port :5100*




