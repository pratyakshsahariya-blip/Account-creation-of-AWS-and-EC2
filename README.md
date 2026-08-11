# Account-creation-of-AWS  

Step 1 : Install & Start Apache Web Server

  1. Update Package Lists :
       sudo dnf update -y
     
  2. Install Apache (httpd) :
       sudo dnf install httpd -y
     
  3. Start The We Server & enable it to launch automatically on boot :

       sudo systemctl start httpd
     
       sudo systemctl enable httpd
<img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/3beda8d5-43f4-4d36-9543-9efe037f9666" />
<img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/e2039202-3e0c-4b47-a333-f1f3037ddeb5" />
<img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/300feef1-39d5-40ba-a7b3-ae0f41f62848" />
<img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/8a9084b6-8ca8-4e6c-9c3c-a9042afcb0bd" />

Step 2 : Creating Website Page

      sudo nano /var/www/html/index.html

      "<h1>Hello, Welcome to my website on AWS EC2!</h1>"
<img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/67053314-2858-4a81-a80d-a243e07b3a48" />
<img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/b4aff78d-05da-4114-b3c8-f38861810431" />
<img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/51496d5d-bdf5-4efc-8054-c357bac195c6" />


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

    <img width="1440" height="900" alt="Screenshot 2026-08-10 195739" src="https://github.com/user-attachments/assets/aee02e4a-2863-45a4-bd90-97f424ba2a09" />

    
    http://13.217.143.64
    
    <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/7f252cd2-15d0-415d-9518-a7864c971ca5" />

