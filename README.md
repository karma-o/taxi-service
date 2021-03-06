# taxi-service
***
This is simple application made for educational and demonstration purposes. Implements authentication by filters based on session. Logs some Authentication information and create/update/delete database operations to console and ```.log``` file. Registration of new drivers, managing the relations between cars, drivers and manufacturers and other CRUD operations.  
Program has next functionalities:
- create new Manufacturer
- display all Manufacturers
- create new Driver
- display all Drivers
- create new Car
- display all Cars
- add driver to car
- list all cars by driver

You can access all of them from the main ```(aplication context)/index``` page  
after registering as a new driver at ```(application context)/drivers/add``` page  
and signing in at ```(application context)/drivers/login``` page (to which you will be redirected if you will try to access pages that are not allowed for unsigned drivers).  
After that you will have access to all the pages and functionalities.

---
## Architecture
1. DAO - Data access layer
2. Service - Application logic layer
3. Controllers - Presentation layer
---
## Technologies
- Java 11
- Apache Maven
- Apache TomCat - version 9
- Apache Log4j2 - version 2.17.1
- MySQL
- JDBC
- Http Servlet
- JSTL - version 1.2
- JSP
- HTML, CSS, XML
 
Update maven dependencies in case you are using any other version of the listed technologies.

---
## Steps to reproduce
*WARNING* Installed TomCat and MySQL is compulsory for this project.
1. Add a tomcat local configuration in IntelliJ.
2. Run SQL script located in ```src/main/resources/init_db.sql``` to set up a database for this project.
3. Configure ```src/main/java/taxi/util/ConnectionUtil.java``` with your ```URL```, ```USERNAME```, ```PASSWORD``` and ```JDBC_DRIVER```.
4. In the ```src/main/resources/log4j2.xml``` at line 7 you also need to set ```ABSOLUTE_PATH``` to your ```.log``` file.

---
## Your database should look like this

![Alt text](readme.images/taxi-database-image.png?raw=true "Database")

---
## Contacts
My [LinkedIn](https://www.linkedin.com/in/vadym-turchenko-6b5884209/)  
I am open for new opportunities as Junior Java Developer