Sypex Dumper 2.0.11 functioning on PHP 7.0 with functions of Mysqli extension. 
Old mysql_* replaced to mysqli_* functions. 

Was changed index.php. You can replace only this file without replacing all files.

Requirements:

Set chmod 777 for ‘backup’ directory.

Set chmod 666 for files ‘cfg.php’ and ‘ses.php’.



If using not default mysql port (not 3306) to make testing for verification correctly of work.


If Sypex Dumper does not work correctly, in index.php do replace:

line 15: //error_reporting(E_ALL);

line 16: error_reporting(0);

to

line 15: error_reporting(E_ALL);

line 16: //error_reporting(0);

If errors are not displayed, to add: ini_set('display_errors', 1);
