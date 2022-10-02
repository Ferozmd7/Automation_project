# Automation_project
prerequites to run the script:-

             ubuntu 18.04 LTS,

             s3 bucket 


1) This script will first do update by "apt update" command.

2) Then it will check for apache2 is installed or not. if it is not installed it will install for us.

3) It will checks the status of apache2 if it is "running" proceed further. if not restart apache2 server.

4) In order to maintain apache2 running after restarts or reboot of system. let's enable it. if not enabled.

5) it will collect the logs in /var/lib/apache2/ make a tar folder using all .log files and save it in /tmp folder.

6) store the tar files in s3 bucket.

7) It will display the logs as using inventory.html


   Log Type    Time Created    Type    Size

   httpd-logs  23092022-114221 tar    4.0K

   httpd-logs  23092022-115517 tar    4.0K

   httpd-logs  23092022-115618 tar    4.0K

   httpd-logs  26092022-165035 tar    4.0K

   httpd-logs  26092022-165138 tar    4.0K


8) it will schedule a cronjob for us.


----------------------------------> happy learning <-----------------------------------------------
