# Codepath_week9
Blue
Vulnerability: Session Hijacking
![Session Hijacking Blue](https://user-images.githubusercontent.com/76242390/114953834-24db1380-9e0e-11eb-8727-c84e2bfe789c.gif)
I opened the same blue websites on Google Chrome and Firefox. Google chrome was not logged in but firefox was logged into the website and by copying the session ID from Firefox I was able to change my session ID on Google Chrome and it automatically logged me into the account.

Blue Vulnerability: SQL Injection
![SQL Injection Blue](https://user-images.githubusercontent.com/76242390/114954009-7f746f80-9e0e-11eb-8728-faeb537d45dc.gif)
I was able to input my SQL injection into the URL https://35.184.88.145/blue/public/salesperson.php?id= and add ' OR SLEEP(5)=0--' to the end of the URL and I was able to pause the page for 5 seconds which shows that my SQL injection worked correctly.

Red
Vulnerability: Insecure Direct Object Reference
![Insecure Direct Object Reference Red](https://user-images.githubusercontent.com/76242390/114954262-0295c580-9e0f-11eb-92be-cced51db296a.gif)
I was able to able to find the IDOR vulenrability by successfully displacing a user account that should not be visible by changing the ID # in the following URL https://35.184.88.145/red/public/salesperson.php?id=1 to https://35.184.88.145/red/public/salesperson.php?id=10 which displays a user account that should "not be public until sept 1". Therefore my IDOR attack was successful. The Blue and Green websites would take me back to the main page whenever I would try to use the same attack on those sites.

Red Vulnerability: Cross-Site Request Forgery







Green
Vulnerability: Username Enumeration
![User Numeration Green](https://user-images.githubusercontent.com/76242390/114954563-bb5c0480-9e0f-11eb-872c-d5f61a6bd894.gif)
In the gif, you can notice that when I try to log in with the username "Raman" who is not a user it displays "<span class="failed>Log in was unsuccessful.</span> but when I use the username "Jmonroe99" who is a user then it displays <span class="failure>Log in was unsuccessful.</span> which shows that the username Jmonroe99 is correct but the password is wrong. Therefore, it has a username enumeration vulnerability.

Green Vulnerability: Cross-Site Scripting
![Cross-Site Scripting Green](https://user-images.githubusercontent.com/76242390/114954939-72f11680-9e10-11eb-95c2-6b24c7299c3c.gif)
A person can post java script in the "Feedback" section as the following <script>alert('Raman found the XSS!');</script> and this java script is executed as soon as the admin logs in and opens the "Feedback" page and the windows pops up displaying the message "Raman found the XSS!.



