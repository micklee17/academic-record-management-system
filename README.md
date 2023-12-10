# Academic Record Management System
System developed by group 17
## Development environments
Windows 10  
Tomcat 8.5.29  
JDK 15.0.x (tested on 15.0.1 and 15.0.2)  
Spring Boot 2.0.1  
MAVEN
## IDE used
VS Code
## Installation
To host the app on your local machine, please follow the procedures below: 
1. Run sql file    
2. ...
3.     

You can log in to the system by using the default credentials
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
