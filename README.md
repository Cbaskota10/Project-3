# User log
**Chabi Baskota & Abdul Basit Razack**

We created different flow charts for the different codes of the application to analyze log in information. We broke up the flow charts into parts to make everything easy and smooth as possible.

The suspicious activity flowchart checks for any unanticipated logins (e.g., between 12:00 AM to 5:00 AM or if the user has logged in more than 5 times on a. given day. If any of those cases are. true, the system will deny the login to the user. 

The system glitch flowchart outlines how the number of logouts will detect glitches. If the number of logouts is more than the number of logins, it will be marked as a glitch. A report will be created to count the total number of glitches once a. day (e.g., one glitch a day accounts for a.  total count of one).

Domain count basically checks the domain of users and records each unique (different) domain in a list. First, it checks the second part of the email using split(). Then, it makes a list of the unique domain, but each domain only occurs once in the list. And also records thhe number of users on each domain. 

Finally, the irresposible behavior checks if the number of logins is more than the number of logouts. This is when user does login but does not log out. If the number of logins is more than the number of logouts, a reported will be created with time, activity, and server informaiton for the logged in user. It will also be sorted on theh basis of time. Then finally, the report will be stored and sent back to the admin. 


