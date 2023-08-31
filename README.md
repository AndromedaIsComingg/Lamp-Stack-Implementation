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
