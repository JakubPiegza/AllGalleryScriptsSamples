Short Powershell script to export user licenses and services' provisioning status.

 

The script is a variation on Get user licenses and services' provisioning statuses . It accounts for the fact that one user may have more than one license assigned and creates records per given user's license.

That means that in the exported csv file, a user with 2 licenses will appear twice, like this:

 

 

 

 

 

How to use?
 

1. Download and run the script.

2. During execution it will ask you for Office 365 Admin credentials

3. If you want to create a report on the users (apart from seeing the info on the screen also export data to a csv), there is a built-in function in the script, and you just need to update the following line:

 

 

PowerShell
$CSVPath="C:\Users\Arletka\Documents\usss34.csv" 
 
 

Expected results
 

During script execution:



 

 

In a csv file:



 

 
