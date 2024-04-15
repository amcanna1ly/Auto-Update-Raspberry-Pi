# Auto-Update-Raspberry-Pi
Automatically updates Raspberry Pi using a script and Cron


Adjust Permission to Allow Execution:
chmod +x update.sh

Set Up Cron:

crontab -e

0 0 * * SAT sh /home/pi/update.sh 2>/home/pi/logs/cronlog

In order to redirect STDERR you have to specify “2>”

This is handy when writing crontab expressions:

https://crontab.guru/
