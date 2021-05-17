# Samogies_LaravelEdition
same project but using laravel

# Samogies
---------------------PRE REQUISITES ---------------------------

you need a Database connection, we used mySql workbench.

Create a database And or configure the connect_Sqli.php and Connect_SamPer.php .

Alter the following files and their Variables as nessessary

connect_Sqli.php{ (SQLI)

  $dbhost = 'localhost:3306';
  
  $dbuser = 'root';
  
  $dbpass = '';
  
  $db     = 'php_samper';
  
}

Connect_SamPer.php{ (PDO)

$mySqlhost  = "localhost:3306"; //127.0.0.1

$username   = "root";

$password   = "";

$myDB       = "php_samper";

}

Run the Sql CreateMenu and CreateUser Table Scripts in XAMPP, These are in the SQL_SamPer folder.
if you ran the previous project and already created the tables, then you should be fine.

Confirm the 2 tables are made in the New or Existing database.
Confirm menus_tbl is filled out.

------------------------------Laravel Specific-----------------------------
Open the 5 php scripts in view and change the path on the includes. they are surronded by comments to catch your attention.
Open the 4 php scripts in the SQL_SamPer folder and change the paths for the includes. they are surronded by comments to catch your attention.

------------------------------Start----------------------------------------

Register-> You must fill in the form completely

on submit will add it to the user_tbl in the database

*note password will be encrypted


Login-> login with username and password 

on submit will check Credentials with the DB

*note will redirect you to the store


Store-> will display products prices descriptions from the database menu_tbl

User will be able to select quantities from both Samosas and Perogies


Confirm-> will display cart items and quantity with total price

*note will send an email to the user logged into the site with by SESSION


Mail-> will email the user a receipt 

displays a thank you message

