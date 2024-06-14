# Working Links
- **Website Link** : <a href="http://52.136.116.225/City%20hospital%20management%20service/" rel="nofollow">City Hospital Management Service</a>
- **Project Video** : <a href="https://drive.google.com/file/d/1g3A2G105p5Ts1O9QPhVU-khmpqjW1i-T/view?usp=sharing" rel="nofollow">Video</a>
- **Project Documentation** : <a href="https://drive.google.com/file/d/1aPbakzsa6-G7Z8WERGJCZ76n6Vyv9FAu/view?usp=sharing" rel="nofollow">Documentation</a>

#  City Hospital Management Service 

The aim of the "City Hospital Management System" project is to revolutionize the way hospitals interact with their patients and staff by leveraging modern technology such as Azure services like AI ChatBot, Azure Web App, and more. These technologies alleviate the load on the developers and create a system that is user-friendly and reliable. The primary goal is to streamline the management of hospital operations, including patient admissions, scheduling, and medical records management, while offering a seamless experience for staff and patients alike. By developing an intuitive online platform, City Hospital aims to enhance patient satisfaction, improve operational efficiency, and drive growth for healthcare facilities.

## Features

- **Azure Virtual Manchine**: To create and host the website.
- **Azure BackUp Service**: To create a Backup of our Web App.
- **Azure Storage Service**: To store backup files.
- **Azure Monitoring Service**: To monitor the usage

## Azure Cognitive Services

This project utilizes Azure's AI Service for the following functionalities:
- **Query ChatBot**: Taking queries from the user and giving proper responds to there queries.

### Prerequisites

- Azure subscription and access to Azure Cognitive Services.
- Azure Virtual Machine With XAMPP to host the application files.

## File Structure

- `index.php`: The main PHP file containing the structure of the web application.
- `styles.css`: The CSS file for styling the application.
- `script.php`: The JavaScript file containing the logic for interacting with Azure Cognitive Services.

## Usage

1. **Book Appointment**: Click on "Book Appointment" to add appointment details inside the hospital data.
2. **Patient Login**: Click on "Patient Login" to go to the personal user dashboard and do further operations.
3. **Doctors Login**: Click on "Doctor Login" to go to the personal doctor dashboard and do further changes in appointments.
4. **Admin Login**: Click on "Admin Login" to go to the admins dashboard where admin can find and manage all the details of hospital management.
5. **Chat With Us**: By scrolling down we get one ChatBot AI where we can write our queries which give us satisfied reply.

## Resource Visualizer

![Computer Vision](https://github.com/shraddhasutar22/CityHospitalManagementService/blob/master/images/Project%20Visualizer.jpg?raw=true)

## Deployment Steps

Search for City Hospital Management Service on Azure portal.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/1.png?raw=true)

Click on create to create new resource.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/2.png?raw=true)

Fill all the required information as shown and click on Review + Create.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/3.png?raw=true)

Once it is deployed successfully navigate to keys and endpoint and copy the key.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/4.png?raw=true)

Paste the copied key in script.js as shown below

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/5.png?raw=true)

Aslo copy the Endpoint URL.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/6.png?raw=true)

Paste the copied Endpoint URL in script.js as shown below 

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/7.png?raw=true)

Then to save the changes click on commit changes with specefic commit message.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/8.png?raw=true)

Now we need to use Azure App Services to deploy our webpage. Search for App Services on your Azure portal.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/9.png?raw=true)

Create a Web App

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/10.png?raw=true)

Fill all the required information as shown below.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/11.png?raw=true)

Select the pricing plan as per your requirements.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/12.png?raw=true)

Now to deploy the project from github navigate to Deployment tab and enable continuous deployment and click on Authorize.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/13.png?raw=true)

Now sign-in to your github account and click on Authorize AzureAppService.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/14.png?raw=true)

Now select your organization, repository & branch and enable basic authentication.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/15.png?raw=true)

And click on create. Once created deployment process will start automatically.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/16.png?raw=true)

Now lets create one storage account which we'll use later for backup purpose of our web app. Search for Storage Accounts on the Azure portal.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/17.png?raw=true)

Fill all the required information as shown below.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/18.png?raw=true)

Now navigate to Advanced tab and click on "Allow enabling anonymous access on individual container" for anonymous access.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/19.png?raw=true)

Now click on review + create.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/20.png?raw=true)

Now we need to create one container to store our backup files. Follow the steps shown below.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/21.png?raw=true)

Now go back to App service and in settings click on backups and select the storage account and the container which you have created earlier and set the backup schedule as per your requirements. 

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/22.png?raw=true)

Now to get alert whenever the App service is restarted. Search for Monitor on the Azure portal. 

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/23.png?raw=true)

Click on Alerts and create new alert rule.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/24.png?raw=true)

Select your web app from the resource group and click on apply. 

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/25.png?raw=true)

Now navigate to condition and from see all signals search for "Restart web app" and click on apply.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/26.png?raw=true)

Now navigate to Actions and create new action group.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/27.png?raw=true)

Fill all the required information as shown below.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/28.png?raw=true)

Navigate to Notifications and add your email and phone number to which alert will be sent and click OK.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/29.png?raw=true)

Navigate to details tab name the action rule.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/30.png?raw=true)

Once all done click on review + create and click on create.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/31.png?raw=true)

## Project Demo

Homepage of project

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/32.png?raw=true)

## Features

### 1. Extract Text.

Upload/Capture any image with text in it select the Extract Text feature and click submit and results will be shown below.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/33.png?raw=true)

### 2. Detect Object

Upload/Capture any image with object in it select the Detect Object feature and click submit and results will be shown below.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/34.png?raw=true)

### 3. Add Caption

Upload/Capture any image select the Add Captions feature and click submit and results will be shown below.

![Computer Vision](https://github.com/sahildsouza/vision-compute/blob/main/images/35.png?raw=true)

