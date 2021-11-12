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

   a. If IDE is `Intellij` then the following steps are to be performed to replace the `settings.xml` file.
````
Go to File -> Settings -> Build, Execution, Deployment -> Build Tools -> Maven

The field `User Settings file` contains the path to the settings.xml file

Navigate to the path and replace the settings.xml file with the file available with same name in the repository
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
