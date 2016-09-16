#Needs to happen every M,W,F before noon.
# GTstuff
##Files are sent MWF and need to be uploaded before noon
##Login secure.sharecare.sharefile.com
###go to shared folder 
###dowload IG_report_current day excel.csv file
####rename to InterventionCallCounts_09122016   (The DATE is the number)

###login in to public.sharecare.com
##go into forms, select a form
###in select a form choose "consent for enrollment Control"
##in select fields choose
1. sid
2. email
3. I ackknonwand agree
4. Entry Date
5. Source URl
6. User Agent
##click on download and export
you can say start date is after august 1st
##download consent form for control group

##go into shared analytics folder 
##open previous M,W,F control consent form
##in control_consent form
##insert a new column after column b
###there should be a blank column c now
copy column a (s_id) and paste into column c
now do a vlookup in conent-for-enrollment-control.csv in column a,2 (starting on B2) against the control-consent_9324329.csv, 
column b and c - then drag down total
##if you have an N/A find the highest sc-gt# and add 1 to it example sc-gt12 is highest add sc-gt13 in place of N/A
After the vlookup is complete copy column A and do a paste special value  (double click) and choose value.
becuase when you close previous .csv (DONT SAVE!!!) the values from vlookup will be lost  

##Go back to public.sharecare.com
##Export entries select a form
##PPS14 Questionaire
##Select ALL
##DESELECT
##Created BY (User ID), Entry ID, Transaction id, Payment Amount, Payment Date, Payment Status, Post Id, User IP, Survey Total Score
start date is after 08/01
##click download and export file
pps14-questionaure-2016-09-15
this is combination of control group and intervention group
then save the file as All_Survery_ (whatever the date is)

When you have the files (3 files) ready upload to cyberduck
login to cyberduck
open connection
use "SFTP"
stefanie eichner
serena is sending credentials to access server to your email

you will need an 
SFTP path: check email
username seichner3
pass: check email

when you login to server
click on sharecare and drop the 3 files in
the 3 files should be
All_Survey_(date).csv
Control_Consent_(date).csv
InterventionCallCounts_(date).csv
