# AdvanceWeb

This project was developed using **HTML5, CSS3, JavaScript, PHP, and MySQL**  
It was created as part of the **Advanced Web Information Systems** course.  

## Installation
1. Download or clone this repository  
2. Place it in the `www` folder (XAMPP) or `www` folder (WAMP)  
3. Create a database in phpMyAdmin and import the `.sql` file  
4. Open the project in your browser via `http://localhost/AdvanceWeb`

Summary of the Login Page 

The Login.php page is designed to handle user authentication for the Grades System. It begins with initializing a PHP session and including configuration, utility, and authentication files. The script retrieves the student_id and password inputs from the login form using a helper function get_or_default. If both values are provided, the system connects to the database with credentials defined in config.php.

A prepared SQL statement is used to securely fetch the record of the student based on the entered student_id. This method prevents SQL injection by binding the input parameter before executing the query. If the execution succeeds, the system checks whether a record exists. If a student record is found, the entered password is compared with the stored database password. A successful match triggers the login() function, which sets the session for the logged-in user and redirects them to view.php.

On the frontend, the HTML displays a simple page with a header, navigation bar, and a login form styled through SiteStyle.css. If login fails, a warning message is shown. Logged-in users see their current status and a logout button. JavaScript validation (validate_login.js) ensures proper input handling before submission.

## Author
- Passwish Kates
