# gas-calendar-accept
Google Calendar Auto-Accept function


Ryan WhealeRyan Wheale
September 2019 edited September 2019
It wasn't obvious to me at first how to use Google App Scripts. Finally found this: https://www.google.com/script/start/



1) Create a new script

2) Copy and paste both the Code.gs file and AutoResponse.html into your project.

https://github.com/ClaudiaJ/gas-calendar-accept/blob/master/AutoResponse.html
https://github.com/ClaudiaJ/gas-calendar-accept/blob/master/Code.gs

3) Go to File -> Project Properties and add a new Script Property named "Id" with your calendar ID as the value (usually your email address - you can find it in your calendar settings).

4) You should now be able to run the script by selecting "ProcessInvites" in the top menu under the "Select function" dropdown and then clicking the play button next to it (note: the play button is disabled until you select an item in the dropdown)

5) If things fail, you can debug yourself. I found the Logger helpful for this. You can view logs by selecting View -> Logs. For example, on line 46 I added this:

```

Logger.log('Found calendar for "' + calendarId + '"');

```

6) If everything works, you can create a trigger by going to Edit -> Current project's triggers and creating a new trigger to kick off your script.



Good luck
