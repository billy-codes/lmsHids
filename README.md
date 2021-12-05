# lmsHids
A host-based intrusion detection system for Learning Management Systems

Important Files:
- hidsconfig.py : Global variables and configuration parameters
- hidsLog       : Format-less log file to store alerts
- idsDB         : HIDS Database to save a list of files in target directory
- lmshids.py    : Main program

Step 1: Setup the configuration file for your program to parse relevant data

Variables and their definitions:
- dir           : Directory of which the web application/software to monitor is stored
- idsDB         : Full Path of HIDS Database directory
- apacheLog     : Full Path of Apache's Log
- lmsAdmin      : Full Path of Web App's Admin page
- lmsTeacher    : Full Path of Web App's Teacher page

Fill out the config file with relevant SMTP information to receive alerts by mail

Step 2: Run the following commands to get the IDS started

` lmshids.py --clear`

`lmshids.py --update`

`lmshids.py --initialize`
