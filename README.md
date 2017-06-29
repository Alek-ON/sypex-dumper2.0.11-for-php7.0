Sypex Dumper 2.0.11 functioning on PHP 7.0 with functions of Mysqli extension. 
Old mysql_* replaced to mysqli_ functions. 

Changed index.php. You can replace only this file. Without replacing all files.


If Sypex Dumper does not work correctly, in index.php do replace:

line 15: //error_reporting(E_ALL);
line 16: error_reporting(0);

to

line 15: error_reporting(E_ALL);
line 16: //error_reporting(0);

If errors are not displayed, to add: ini_set('display_errors', 1);

If using not default mysql port (not 3306) to make testing for verification correctly of work.
