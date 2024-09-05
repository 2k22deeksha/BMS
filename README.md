# BMS
Book My Show - 
Console Application

Project Description:

The project is a console-based application developed to facilitate the booking of tickets for various events. The application allows users to book seats.


User Flow:
1. Clone the repository using:<br>
   git clone https://github.com/2k22deeksha/BMS.git
2. Install the Requirements<br>
   Ensure you have Python installed. Install the required packages by running:<br>
   pip install -r requirements.txt
3. Set Up the Database
   The application uses MySQL for database management.<br>
   a) Download and configure MySQL:<br>
        •   Install MySQL from the official website or through your package manager.    
   b) Update settings.py with your database details:<br>
        •	Enter your MySQL credentials in the settings.py file.
            ![img_2.png](img%2Fimg_2.png) 
   c) Configure MySQL in PyCharm:<br>
        •	Click the database icon in the IDE, select MySQL, and enter your username and password.<br>
        •	Test the connection and click "OK."
            ![img_1.png](img%2Fimg_1.png)
   d) Create the Database and User:   
        •	Open a console session in MySQL and run the following commands:<br>
             CREATE DATABASE database_name;<br>
             CREATE USER 'user_name'@'localhost' IDENTIFIED BY 'password';<br>
             GRANT ALL PRIVILEGES ON database_name.* TO 'user_name'@'localhost';
             ![img.png](img%2Fimg.png)
   e) Switch to the Created Database:<br>
        •	Run the following commands in the MySQL console:<br>
            SHOW DATABASES;<br>
            USE database_name;
4. Generate Database Tables<br>
   Navigate to the project directory and run the following commands to create the necessary tables:<br>
            python manage.py makemigrations<br>
            python manage.py migrate
            ![img_5.png](img%2Fimg_5.png)
5. Run the Application<br>
   Go to the book_my_show directory, open test.py, and execute the script:<br>
            python test.py
            ![img3.png](img%2Fimg3.png)           
You can now see the status of your ticket on the console, and the database will be updated accordingly.<br> 

Technology Stack<br>
•	Backend: Python, Django Framework<br>
•	Database: MySQL


