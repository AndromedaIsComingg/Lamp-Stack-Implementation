# Lamp-Stack-Implementation
Project 3


## AWS Account & EC2 Instance
###### Created an AWS Account and spinned an EC2 instance name "For Instance"
<img width="1280" alt="AWS Acct" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/14e2925b-50d3-4442-8bae-1dbc8768da8a">


## Private Key
###### Created and downloaded a private key named "1stkey"
###### The .pem file was saved in the download folder

<img width="320" alt="pem file in dwnlds" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/d73e3fac-39ac-42ef-a5d3-844018d53cbe">


###### From Terminal, working directory was changed to the download folder
<img width="272" alt="cd Downloads" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/f0d64650-0ac8-40d6-b2ae-5177940e2a91">

###### From Terminal, permission was changed for the private key.
<img width="412" alt="changing permission for private key" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/6890a6f6-da94-49d0-a2e5-cc5894f8888d">

## Connecting to the EC2 Instance
###### Connected to the EC2 instance by running the command "ssh -i <private-key-name>.pem ubuntu@<Public-IP-address>"
<img width="598" alt="starting ubuntu" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/26d1bd55-66c9-4463-b6f2-404f2108b137">


## Installing Apache & Installing Firewall
###### Updated a list of packages in package manager
###### Updated these packages with the with the command "sudo apt update" with the "sudo giving admin privelages.
###### After which the Apache package was installed using the "sudo apt install apache2" command
<img width="735" alt="sudo apt and apache2 instl" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/f4be9849-17c6-444a-ba45-67d2d818a64e">


## Verifying Apache
###### Verified that Apache was running as a service in the os with the command "sudo systemctl status apache2"
<img width="653" alt="apache2 verifucation" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/9d7c1cd6-cd36-4dbe-b7ac-fb0a8565d137">


## Editing Inbound Rule
###### Edited inbound rule such that connection through port 80 is allowed and from any ip address.<img width="1271" alt="editing inbound rule" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/b90f17dd-51aa-422a-a2e3-f19a52b4b278">


## Accessing Server
###### Accessed server locally on Ubuntu shell using the curl command
<img width="917" alt="curl local host check" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/127203f3-61eb-4eb9-bd9b-15acc62df7e5">

###### Tested the Apache HTTP Server with a web browser. This done by using the public ip in the address bar.
<img width="949" alt="apache test web" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/93072342-9964-44ef-9034-5f8a25c2bc64">


## Installing Mysql
###### Used apt to install this software using the command "sudo apt install mysql-server"
###### The sudo command gives admin previlages and when prompted, installation was confirmed by typing y and then pressing enter.
<img width="1222" alt="sudo MySQL install" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/82feb343-7c33-4cce-851c-0a29fd3d31df">


###### After installation, logged into the Mysql Console with the command "sudo mysql"
<img width="561" alt="MySQL Start up" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/605ca9d8-7387-493e-ab01-18536f1da7bd">


##### Password was set for root user using the command "ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'PassWord.1';"
<img width="661" alt="user password" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/a8c63d47-187a-4499-8b24-adc24fe7a93e">


##### When done, test to login into the MySQL console by using the command "sudo mysql -p"
##### The -p flag prompts for password after the root user password has been chnaged.
##### The "mysql> exit" command was used to exit the MySQL console.

<img width="580" alt="login test   exit" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/ed835c52-1429-4213-b3a9-4c8eac184d0c">


## Istalling PHP
##### In order to proccess codes to display dynamic content to the end users, PHP is the package to install.
##### In addition to PHP, we install other features like, php-mysql and libapache2-mod-php
##### These 3 packages were insatalled at once with the command "sudo apt install php libapache2-mod-php php-mysql"
<img width="1082" alt="PHP   co install" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/ccc93fde-09c5-4c14-9e81-59d20cbb1670">

##### Afterwhich the version of PHP was confirmed using the command "php -v" and the verision is 8.1.2
<img width="563" alt="PHP version" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/06ad99df-10a1-4037-8dfa-af2760f14958">


##### Changing the order of files in the default directory index such that index.php file will take precedent over index.html
##### This was done using the command "sudo vim /etc/apache2/mods-enabled/dir.conf"
<img width="715" alt="Vim command" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/54b1ced0-0364-499c-a80a-0967edce9611">


##### This order was edited using the insert mode "i" in the vim editor.
##### Chnages were written and vim was exited with the command ":wq!"
<img width="708" alt="Vim" src="https://github.com/AndromedaIsComingg/Lamp-Stack-Implementation/assets/140917780/ec0e8c3e-ae9e-4bde-8897-e999fe2f2fe8">




