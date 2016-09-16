#Needs to happen every M,W,F before noon.
# GTstuff
##Files are sent MWF and need to be uploaded before noon
##Login secure.sharecare.sharefile.com
###dowload excel.csv file
####rename to InterventionCallCounts_09122016   (The DATE is the number)

###login in to public.sharecare.com
##go into forms, select a form
###in select a form choose "consent for enrollmetn"
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

##open up previous Control_Consent
##in control_consent form
##insert a new column after column b
###there should be a blank column c now
copy column a (s_id) and paste into column c
now do a vlookup in conent-for-enrollment-control.csv (starting on B2) against the control-consent_9324329.csv

##Go back to public.sharecare.com
##Export entries select a form
##PPS14 Questionaire
##open up All_Surver_(the date)
##Select ALL
##Created BY (User ID), Entry ID, Transaction id, Patment Amount, Patment Date, Payment Status, Post Id, User IP, Survey Total Score
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
