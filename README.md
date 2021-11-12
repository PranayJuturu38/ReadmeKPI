# Kpi-reports-api
***
## Prerequisites
* Spring Boot - v2.0.1.RELEASE
* Maven - v3.8.1
* Java - v8
* MYSQL Server - v5.7.33

## Description

KPI-Report-API repository consists of two java based projects based on adapter desgin pattern.The report REST API application handshakes with the front end application. 
The report application is used as an internal dependency which does the heavy lifting for report module.

The application can be accessed through the link below
````
https://universe-report-v4.testing.kpininja.com/#/reports.
````

## Steps to install and run
1. Clone git reposotiry
````
git clone https://bitbucket.org/kpininjarepo/kpi-reports-api/src/dev/
````
2. Replace settings.xml file

   a. Steps to replace `settings.xml` in `Intellij` IDE
   ````
   * Go to File -> Settings -> Build, Execution, Deployment -> Build Tools -> Maven
   * Select the 'Override' checkbox next to 'User Setting File'.
   * Click on Browse button and select the settings.xml file from the repository.
   * Click Apply.

   ````
   b.Steps to replace `settings.xml` in `Ecllipse` IDE
   ````
   * Go to Window -> Preferences
   * Click on the Browse button of User Settings, and select the settings.xml from the repository.
   * Click on the "Update Settings" button to update the settings. If any confirmation dialog appears, just click Yes.
   
   ````
3. Navigate to the folder where the repository is cloned and run the following command to build the application.
````
mvn clean install
````
4. Run the application using the command
````
mvn spring-boot:run
````
## Sample URL
Following url is a sample url for the kpi-report-api
````
http://localhost:9196/report/reports?type=global&modules=&search=&sortType=&sort=&page=1&limit=10
````
## Postman Collection Link
The Postman collection link is used to test the endpoints and perform request mapping.
````
https://www.getpostman.com/collections/4849ea95277297af6c98
````

###Author
[Pranay Juturu] (pjuturu@kpininja.com)

