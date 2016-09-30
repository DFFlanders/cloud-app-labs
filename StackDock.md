Happy Birthday, OpenStack

The Lab:
Tenants for participants:
User: user<n>@osbday.hackathon ( <n> - digit 1 - 10 )
Example: user1@osbday.hackathon
Password: WeAreTheOpenStack2016
URL:
https://somedc.com/


Murano Mini hackathon Plan

After this hackathon you’ll get familiar with OpenStack Murano and App Catalog, learn to install and deploy Murano Apps in the cloud, write your own application which deploys application in the cloud from Docker image picked by you.

Getting acquainted with Murano

Load application from the catalog
Open apps.openstack.org. https://apps.openstack.org/
Look for Docker Nginx. Copy link to zip file with the package
Import the application into the cloud
Login to the cloud (address+name+password are provided by organizers)
Menu item Murano\Manage\Package Definitions
Button “Import Package”
Import via url
Check that packages of the app are downloaded (Murano\Manage\Package Defenitions) and images OS (Murano\Manage\Images)

Deploy the application Nginx
Open menu Murano\Application Catalog\Environments
Push button “Add New” and create new environment
Add application DockerNginx
“Container Host” -  choose Docker Standalone Host and press Next
“Instance flavor” -  choose M2.Medium.4
“Instance Image” -  choose Ubuntu
Don’t change other fields
Press Create
Once again press Create
Press “Deploy this environment”
Wait for application to complete
Go to Project/Compute/Instances and check that your application has started a new virtual machine for you
Find address of the new virtual machine, open it in the browser
Welcome to nginx!




Creating new application using Docker image
Before passing on to the next stage of hackathon delete environment created before.

Choose the docker image based on which we want to make the application

Product being deployed
Image name
jenkins
jenkins
joomla
'gjong/apache-joomla'






you may choose another one after consulting the mentor
Download an archive of the application to be modified
Go to menu Murano/Package Definitions
Find package Docker Nginx.
Press Download Package. Download
Unpack the Archive
Modify the initial code
Edit file DockerNginxSite.yaml, Rename into MyFirstApp.yaml
In line №18 change class name into MyFirstApp 

https://github.com/openstack/murano-apps/blob/stable/kilo/Docker/Applications/Nginx/package/Classes/DockerNginx.yaml#L18
In line №42 change the image name nginx into the one chosen by you
In line №46 change port into 8080 
In lines №61 and №63 change Nginx into the chosen by you image. These messages are displayed on installation
Edit UI/ui.yaml
In line 17 change com.example.docker.DockerNginx into 
com.example.docker.MyFirstApp

https://github.com/openstack/murano-apps/blob/stable/kilo/Docker/Applications/Nginx/package/UI/ui.yaml#L17
In line 34 change
initial: DockerNginx
into
initial: MyFirstApp


Edit manifest.yaml
Change package name into
FullName: com.example.docker.MyFirstApp


Rename to MyFirstApp
Change the description (поле Description) into the one you like
In line №22 rename file name and class.example.docker.MyFirstApp: MyFirstApp.yaml

https://github.com/openstack/murano-apps/blob/stable/kilo/Docker/Applications/Nginx/package/manifest.yaml#L22
Optional - change the logo
Pack updated file into archive
Download the renewed application into the cloud
Open Horizon, menu Murano/Package Definitions
Press “Import Package”
Select archive with updated files
Next
Next
Create
Check that your new package MyFirstApp is there in the list

Create environment and deploy application as we did it before in #2
“Deploy this environment”
Wait for application to complete
Go to Project/Compute/Instances, check that your app started new VM for you
Find address of the new VM and open it in browser using port 8080 or 80 (depends on image you choose)
You should see an interface of your new app




