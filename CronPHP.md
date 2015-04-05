# Introduction #

How to set cron to run the todatabase.php and chart\_upload.php files and get the weather charts on an online server every hour.

THIS is for use with a Linux Server (cron jobs on windows are done another way)

# Details #

From http://www.htmlcenter.com/blog/running-php-scripts-with-cron/

First, you need access to Lynx (Lynx Browser for more information). Lynx is a small web browser, generally available on Unix and Linux.

Running your PHP script will not require you to add any additional lines. You simply have to edit your /etc/crontab file and add the following line:

lynx -dump http://www.somedomain.com/cron.php
Please note that in general, you have to specify the entire URL (with “http://” and so on). But depending on your Lynx’s configuration, the URL might be relative; I suggest always using the absolute reference as in my example above – it always works.

Again execute the following from the command line:

Shell> crontab crontab