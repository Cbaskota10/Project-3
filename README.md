# User log
**Chabi Baskota & Abdul Basit Razack**

We created different flow charts for the different codes of the application to analyze log in information. We broke up the flow charts into parts to make everything easy and smooth as possible.

The suspicious activity flowchart checks for any unanticipated logins (e.g., between 12:00 AM to 5:00 AM or if the user has logged in more than 5 times on a. given day. If any of those cases are. true, the system will deny the login to the user. 

The system glitch flowchart outlines how the number of logouts will detect glitches. If the number of logouts is more than the number of logins, it will be marked as a glitch. A report will be created to count the total number of glitches once a. day (e.g., one glitch a day accounts for a.  total count of one).

Domain count basically checks the domain of users and records each unique (different) domain in a list. First, it checks the second part of the email using split(). Then, it makes a list of the unique domain, but each domain only occurs once in the list. And also records thhe number of users on each domain. 

Finally, the irresposible behavior checks if the number of logins is more than the number of logouts. This is when user does login but does not log out. If the number of logins is more than the number of logouts, a reported will be created with time, activity, and server informaiton for the logged in user. It will also be sorted on theh basis of time. Then finally, the report will be stored and sent back to the admin. 

# Issues faced while coding this project

We faced some issues while coding this project. The first in the very begining while trying to open file. We had the correct code, however, it was not working for some reason. We reached out to the TA's and professor on discord and they helped us with it. The problem was that we had to delete the userlog.log file and redownload it about three times before it finally worked. The code for it was: open_file = open("userlog.log", "r")

Another issue was with the domain count part. We did not set our for statement properly while coding the domain count part. Initially, we had: for "x" in range(int.len(logs)/5). That was wrong and we seeked help from our TA to get the correct code which was: for x in range(int(len(logs)/5)):. There was a mistke with the period in between the "int" and "len". There was also parenthesis missing in between that. 

The next issue was the split operator not working properly. First, we had:

for line in open_file:
    print(email)
    email = username@domain.com
    print(email.split(" @ "))[1]
    splits = username()
    
It was completely wrong and we had to seek to our TA's again for why the split function was not working properly. After consulting with them, we came up with:

for line in open_file:
    print(line)
    email = ".com"
    print(email.split(" @ ")[1])
    splits = email.split()



# Description of Implementation

For all four analyses, we used a for loop " for x in range(int(len(logs)/5)): ". Then defined email as "email" then counted the logs using " count = count+1 ". We used x and y in for loops to implement the rest of the analyses. 
Finally, we printed it into a new log file by first telling python to create a new notebook, then using. 
For all four analyses, we used a for loop " for x in range(int(len(logs)/5)): ". Then defined email as "email" then counted the logs using " count = count+1 ". We used x and y in for loops to implement the rest of the analyses new_file_name.write code to write it on to that new file for each report. 




