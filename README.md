# MacOS-Notify-Script
Tired of running big jobs, browsing the internet while waiting, and then not noticing when the job is complete! This bash script gives a nice little notification complete with icon, sound, and unobtrusive notification popup. 

![Success notification](https://i.imgur.com/J4UK78z.jpg)

![Fail notification](https://i.imgur.com/AbfCAFm.jpg)

To add, copy the notify folder to your computer and add the following to your bash profile:

```
notify_script_location="~/Documents/scripts/"


alias success="open $notify_script_location/notify/success.app"
alias fail="open $notify_script_location/notify/fail.app"

alias notify="success || fail"
alias n="success || fail"
```
This software is only available on OSX.


Remember to set the notify_script_location in the bash profile.

Then, run bigjob && n to recieve a notification!
