# MacOS-Notify-Script
This script notifies you when a job is complete with a OS notification center notification, an OS notification sound, and a matching success/fail icon.

![Sample image](https://i.imgur.com/J4UK78z.jpg)


To add, copy the notify folder to your computer and add the following to your bash profile:

```
notify_script_location="~/Documents/scripts/"


alias success="open $notify_script_location/notify/success.app"
alias fail="open $notify_script_location/notify/fail.app"

alias notify="success || fail"
alias n="success || fail"
```

Remember to set the notify_script_location in the bash profile.

Then, run bigjob && n to recieve a notification!
