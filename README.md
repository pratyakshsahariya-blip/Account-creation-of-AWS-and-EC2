# Account-creation-of-AWS  

Step 1 : Install & Start Apache Web Server

  1. Update Package Lists :
       sudo dnf update -y
     
  2. Install Apache (httpd) :
       sudo dnf install httpd -y
     
  3. Start The We Server & enable it to launch automatically on boot :

       sudo systemctl start httpd
     
       sudo systemctl enable httpd

Step 2 : Creating Website Page

      sudo nano /var/www/html/index.html

      "<h1>Hello, Welcome to my website on AWS EC2!</h1>"

Step 3 : Opening HTTP Traffic in AWS Console 

  1. Opening a new browser ta and go to the AWS EC2 Management Console.

  2. Go to Instances and clicking on instance (i-07ec044d333ff2fb1).

  3. Selecting the Security tab near the bottom.

  4. Clicking on the Security Group link listed under Security groups.

  5. Clicking on Edit inbound rules.

  6. Clicking Add rule and setting :
     . Type : HTTP
     . Port Range : 80
     . Source : Anywhere-IPv4 (0.0.0.0/0)

  7. Clicking Save Rules.

Step 4 : Viewing Our Website :

  Opening a new browser tab and going to our Public IP address :
  
    http://54.196.62.205
