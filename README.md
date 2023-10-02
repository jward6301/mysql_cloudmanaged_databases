# mysql_cloudmanaged_databases
HHA 504 Week 4 Assignment

## Azure:
1. Log into Microsoft Azure using the following link: https://azure.microsoft.com/en-us/get-started/azure-portal
2. Once logged in, click on create a resource
3. Search in the search bar “Azure Database for MySQL” and click on it to open
4. Once the option is open, click on the create button
5. Click on the create button under the flexible server option
6. There will be 4 different sections to work through: basics, networking, security, tags and review + create
7. Under basics, the project details should  be selected to Azure for Students under Subscription and under resource group select create new and name according to your project. Mine was named Jessica504-wk4. The service details should be: server name as hha504wk4, region should be set to East US and select the workload type. Under compute + storage, I selected the burstable tier and set up admin user.
8. Next, click on the Networking tab. The connectivity method should be selected to Public access. Under firewall rules, the option for allowing public access should be checked off. Add a firewall rule and enter the following information AllowAll under rule name, start IP address as 0.0.0.0 and the end IP address as 255.255.255.255.
9. For my project nothing was needed for the remaining sections for review + create was moved onto. If all information is correct, you can select Create. 
10. Connect MySQLWorkbench to Azure

##GCP
1. Log into the Google Cloud account using the following link: https://console.cloud.google.com/
2. Select the dropdown next to GoogleCloud and select New Project on the right side
3. Once the page loads, create a project name, select the appropriate organization and location it will be attached to. Once thsoe are all selected click create
4. On the menu on the left hand side, click SQL.
5. Click on create instane and click on MySQl on the popoup.
6. The following options should be selected on the page, MySQL8.0 under database version, Enterprise under Cloud SQL Edition, Sandbox under preset for this edition, and a shared core with 1vCPU/.614gb RAM selected. Public IP addresses should be enables and add a authorized network with the name as AllowAll and the IP address should be set to 0.0.0.0/0
7. Click create
8. Connect MySQLWorkbench to GCP
* These steps were followed during lecture with Professor Williams

## My experience with MySQL Workbench
My experience with MySQL Workbench was fairly easy as Professer Williams went over the necessary steps in class. I used the code copied here https://github.com/jward6301/mysql_cloudmanaged_databases/blob/main/sql.sql in MySQL Workbench. The tables and code were the same for both GCP and Azure. 

## Errors or Troubleshooting
I had some issues connecting the MySQLWorkbench to Azure, as I was originally following the steps completed in class to connect it to GCP. I followed the steps on the following link and was able to connect it to Azure : https://learn.microsoft.com/en-us/azure/mysql/single-server/connect-workbench. The difference being that the Hostname for GCO was my IP address and the Hostname for Azure wa created by Azure and provided on the overview page of the resource. 
