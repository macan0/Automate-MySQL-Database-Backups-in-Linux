# Automate-MySQL-Database-Backups-in-Linux
Automate MySQL Database Backups in Linux with Email notifications

1. First run this commands in the linux command line:
sudo apt-get update 
sudo apt-get install postfix mailutils

Then go to your root directory and clone this repository
enter into the new directory
then chmod x backup.sh
then open the backup.sh with :
nano backup.sh
change the username, password, database, email acording to your setup

then just setup this cron job:

sudo crontab -e
30 22 * * * /root/backup.sh
