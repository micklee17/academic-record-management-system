# Academic Record Management System
System developed by group 17
## Development environments
Windows 10  
VS Code  
Tomcat 8.5.29  
JDK 15.0.x (tested on 15.0.1 and 15.0.2)  
MySQL 8.0  
Maven 3.9.6 (tested on 3.9.6 and 3.8.6)
## Frameworks
Spring Boot 2.0.1  
MyBatis
## Installation
Originally, we planned to deploy the app on Heroku, but since now Heroku is not permanently free we can only ask our users to deploy and test the app locally.  
  
To host the app on your local machine, please follow the procedures below: 
1. Create a MySQL database, run the school_record.sql file to create the tables into your database.
   
2. Open the application.yml file and replace the db url, username and password with your own.
![image](https://github.com/micklee17/academic-record-management-system/assets/104964040/5dedfe12-f112-4ccc-b988-8c335c61ad64)  
![image](https://github.com/micklee17/academic-record-management-system/assets/104964040/6dd3efba-17ad-4dcf-b1ec-87f665752d45)
![image](https://github.com/micklee17/academic-record-management-system/assets/104964040/7e6c4448-aa9c-46d0-b8fb-d58f86a9c3c2)

  
3. Run StudentmanagerApplication.java.
![image](https://github.com/micklee17/academic-record-management-system/assets/104964040/ba4762dc-9973-4b34-87c2-6363c4b1a48e)
  
4. Open your browser and go to localhost:8080.
![image](https://github.com/micklee17/academic-record-management-system/assets/104964040/8991c775-288f-4f1c-a00a-677d271fade1)

  
You can log in to the system by using the default credentials.
| User Type      | Account        | Password       |
|:---------------|:---------------|:---------------|
|Admin           |admin           |admin           |
|Teaching Staff  |jauyeung        |jauyeung123     |
|Student         |s1000000        |12345678        |  
  
To create your own testing account, you can insert a pair of username and password into the database by yourself. 
## Problems to be fixed
1. Wrong constraints on email and phone number leading to errors when trying to modify the two attributes. 
2. Admin can set student username that doesn't match that student's SID (i.e., studentID of a student is 12345678, his/her username should be s1234567, but admin can set it to s9999999 for example).
3. Attributes like programme name and teaching staff name are displayed incorrectly on some occasions (will show programme ID/teaching staff ID instead of name).
## Functions to be added in the future
We have only implemented the major functions about operations on academic records, there are still more functions to be added incrementally, including:  
1. Useful links
2. School news
