# DevOps Engineer Portfolio_Webpage on Nginx Server

  -----------------------------------------------About Nginx Server---------------------------------------------------

-  NGINX is a high performance web server developed to facilitate the increasing need of the modern web.
-  It focuses on high performance, high concurrency and low resource usage.
-  It mostly known as a web server.
-  Its core is a reverse proxy server.
-  NGINX  is not only webserver on the market, its a biggest competitors is Apache HTTP server (httpd).
-  NGINX is faster in static content delivery while staying relatively lighter on resources because it dosent embed a dynamic programing language processor.
-  when a request for static content comes, NGINX simply responds with the file without running any additional process. That dosent mean that NGINX can't handle
   request that reqire a dynamic programming languge processor.
-  In such case, NGINX simply delegates the tasks to seprate process such as PHP-FPM. Node.js or Python.

  * Prerequisite
    - Ubuntu SHH Machine - EC2 Instance - Free Tier 
    - HTML Code

  * Steps to be followed :-

    Connect Ubuntu through SHH

    Update the system with command :
         - sudo apt-get update

    Install NGINX in the system :
          - sudo apt install nginx
      
    Check NGINX work perfectly in your system :   
          - systemctl status nginx

    After the check NGINX work properly then restart the NGINX server :
          - systemctl restart nginx (other way to copy public IP address and paste new chrom window, It run by default running prot 80.)
          - E.g. - http://16.171.141.77/

    Go to the below mention path, this path is important part of this project when "index.html" file create in this path then website will deploy on port 80.
          - /var/wwww/html - Root folder

    Create index.html with command :
          - sudo vim index.html

    Note : Before paste the code change some informations about you.
           For better experience and undertand the language open the code on Notepad++.

    HTML code where need to change : Two major changes.
       
       - In Headear section chnage the below details.
                <h1>ZAFAR SAYEED</h1> (write your name here)
		            <h2>DevOps Engineer Portfolio</h2> (Write your profile name here)
		            <p>Showcasing my journey in DevOps</p> (Write anything you want to show on your portfolio)
      
      - In section change your contact details. 
        	<p>Linkedin Id : <a href="www.linkedin.com/in/zafar-sayeed-969840130"> www.linkedin.com/in/zafar-sayeed-969840130 </a></p> (Write your Linkedin Id)
		<p>Gmail Id : <a href="mailto:zafar.sayeed2023@gmail.com">zafar.sayeed2023@gmailcom </a></p> (Write your Gmail Id)
        

    Last Step Refresh your page.

    Congrestulation ! Your Protfolio has been deployed on Nginx server.
    
