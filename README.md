csc450p4
========

CSC450 Project 4: Ring Manager Agent

Create two android emulators.
Start them both.
Let's call them emulator 1 which should be running on port 5554 and emulator 2 which should be running on port 5556.
On emulator 1 create a contact named "Sam" with phone number 5556667777.
Send a geo location of lat 20 and long 20.
On emulator 2 send a geo location of lat 0 and long 0.
Go into Run Configurations -> Target -> Launch on all compatible devices.
Run it.
To set urgency of a call, before "calling" type in "Agent: Important" or "Agent: Casual".
e.g. For Sam to call emulator 1 with an important call, type in "Agent: Important" and call 5556667777 to emulator 1.
That should create a notification on emulator 1.
For Sam to call emulator 1 with a casual call, type in "Agent: Casual" and call 5556667777 to emulator 1.
(Every call is marked as casual by default. So, "Agent: Casual" is unnecessary.)
So, since both are private, they won't check each others locations.
If emulator 1 is public but 2 is private, it will send emulator 2 a location check and emulator 2 won't.
If emulator 1 and 2 are public, it will send emulator 2 a location check. Emulator 2 will send a location. Emulator 1 will receive it and check the distance. If within 50m, emulator 1 will create a notification.

In order to add a calendar (only works with NCSU gmail apparently)
-Open up the calendar
-Attempt to add an entry
-You will get a pop up requiring to add calendar - click ok
-Enter your ncsu email address and password and click next
-After the server retrieves your info, change domain to google\<your ncsu unity id>@ncsu.edu and Password to your ncsu password.
-Change the server to m.google.com
-Scroll down and click next.
-A Remote Security notification displays - click okay
-Select the items you want to sync and click next
-Enter a name for your calendar and click next
-You should receive a prompt to activate device administration. If you
don't see it check your notifications. Click Activate.

Now to check calendar interface make an event that is currently going
on during the check.  It will only check back to midnight for the
current day and it will only check 1 event if they're conflicting. 

