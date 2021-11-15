# Kpi-reports-api
***
## Prerequisites
* [Spring Boot](https://spring.io/) - v2.0.1.RELEASE
* [Maven](https://maven.apache.org/download.cgi) - v3.8.1
* [Java](https://www.oracle.com/java/technologies/downloads/) - v8
* [MYSQL Server](https://www.mysql.com/downloads/) - v5.7.33

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
2. Creating Database
````
create database testing_univ_dev_v4;
````
3. Schema for the database can be found at
````
https://bitbucket.org/kpininjarepo/kpi-univ-sql/src/66ec6080da6608bee7921a161542ef556c827053/Structure%20%26%20Default%20data/?at=release%2Fdev
````
4. Replace settings.xml file

   a. Steps to replace `settings.xml` in `Intellij` IDE
   ````
   * Go to File -> Settings -> Build, Execution, Deployment -> Build Tools -> Maven
   * Select the 'Override' checkbox next to 'User Setting File'.
   * Click on Browse button and select the settings.xml file from the repository.
   * Click on Apply.

   ````
   b.Steps to replace `settings.xml` in `Ecllipse` IDE
   ````
   * Go to Window -> Preferences -> Maven -> User Settings
   * Click on the Browse button of User Settings, and select the settings.xml from the repository.
   * Click on Apply. 
   ````
5. Navigate to the folder where the repository is cloned and run the following command to build the application.
````
mvn clean install
````
6. Run the application using the command
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

### Author
[Pranay Juturu](https://teams.microsoft.com/l/team/19%3aWB7L5KVaUkHBv8UiBt5xM0FMDdQNflVtrAPeXdH0XjI1%40thread.tacv2/conversations?groupId=444694ad-ecca-4857-a955-e3cf09528bd5&tenantId=d07ee4ce-db25-419d-a7d2-b04977af8f2a)
