# CPSC471Project

A cinema theatre website that has three types of users: Customers, Employees, and Managers. 

Customers: A customer is able to register for an account of login using an existing account. Once a customer logs in, they are able to view future Movie Showings (which also displays the name of the Movie, the duration of the Movie, the genre of the Movie, and the location of where the movie is being held) as well as all seats for the Movie Showing that have not yet been reserved. A customer is then able to book seats for the Movie Showing. Once they have booked seats for a Movie Showing, they are also able to order food for Movie Showings that they have reserved. Lastly, a customer can view their account information as well as all of the bookings that they have created. A customer can choose to cancel the food that they have ordered for a Movie Showing or cancel an entire booking for a Movie Showing.

Employees: Employees must first login to be able to view the Food Orders that they need to complete. An employee can change the status of a Food order to In Progress to signify that an order is being worked on or change the status to delievered to signify that the Food Order has been completed. At this point, the Food Order will not be diisplayed to any employee. Lastly, an employee can view their account information.

Manager: Managers are important to the system in that they manage an entire cinema theatre. As a result, they can add or remove Movies from the system as well as Movie Showings. Adding Movie Showings to the system will also add a predetermined number of seats to the system which can be reserved by customers. Removing a Movie Showing will remove all bookings made by customers for the Movie Showing, it will remove all of the seats for the Movie Showing, and it will also remove all Food Orders made by customers for the Movie Showing. Lastly, a manager can view their account information.

The project is separated into two parts: the Project and the Project API. 

Project: The Project folder contains a complete implementation of the system as a website. It uses HTML and CSS to create and format the website and PHP to connect to the database and obtain information. MySQLi prepared statements are used in PHP to insert information into the database or obtain information from the database as well as to prevent SQL injections.

Project API: The Project API folder contains an implementation of only the endpoints of the website system. The Postman tool is used to test these endpoints against the database. The link to the Postmand Documentation is here: https://documenter.getpostman.com/view/18775667/UVRAJ7Ry.

The main part of this project was properly creating a SQL database using techniques such as extended ER diagrams and relational models. The database creation was the intergral part of the project and the website and endpoints revolved around it. The website was created after initally designing it using different types of diagrams such as HIPO and DFD diagrams. Lastly, the API endpoints used basic CRUD operations to have properly functioning endpoints in PHP. 

=========================== Project ===========================

Copy the project folder in www of AppServ (i.e. C:\AppServ\www\Project).

Load the sql file into your database. In the file Project\Database\connection.php,
change the username and password to your own mysql user and password.
$con=mysqli_connect("127.0.0.1", "<username here>", "<password here>").

Open browser and in the search bar type localhost.
Then type Project and the path to the php file name you want to open. (i.e. http://localhost/Project/Customer Login/filename.php).
Below is the paths for the php files you want to execute:

Customer Login: http://localhost/Project/Customer Login/existingCustomerAccountF.php

Employee Login: http://localhost/Project/Employee Login/existingEmployeeAccountF.php
