# AWS FINALIZED PROJECT
# Technology use
Amazon Web Service (AWS) to achieve my project and GIT BASH: for a git command line .
An official VPC and subnets has been created. All i did was to create security group and launch my instances
# Region
The specific region to be use is Ireland, which was specify on the project i am working on. first step is i set my region to IRELAND.
![region](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/region.gif)
# First Step is to create Security Group
Since i want to launch an EC2 instance, first i went to ec2 to create a security group, under EC2 i click on security group and i click on "create security group". Filling the basic details: security group name: containing my name, Description: Allow SSH and HTTP traffic, VPC: selecting the VPC that has already been created by Lita.
![SG1](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/SG%201.gif)
 # Inbound rule
 I added two inbound rules ssh and http traffic
 ![SG2](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/SG%202.gif)
 # Outbound
 The outbound rules has alreadcy been generated through the ssh and http traffic.
 ![SG3](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/SG%203.gif)
 # Successfullly created a security group
 using my name added LitaSG, allow two inbound rules(SSH and HTTP) CUSTOM: Anywhere, using Lita VPC.
 ![SG Launch Successfully](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/SG%20Created%20successfully.gif)
 # Launch EC2 Instances
 Launching of instance, added name, AMI:choosing Amazon Linux 2 AMI, instance type: t2 micro, select existing keypairs that has been created by me, network setting: VPC lita_project, Subnet: lita_project-subnet-public1, Auto-assign public IP: Enable, Security group: select existing one created by me, configure storage: 8 gp2. LAUNCH INSTANCES.
# Name and tag
Containing my name and i added lita at the front.
![Launching EC2 Instances 1](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/Launching%20EC2%20instances%201.gif)
# AMI (Amazon Machine Image)
I choose Amazon linux 2 AMI.
![Launch EC2 Instances 2](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/Launching%20EC2%20instances%202.gif)
# Instances type
instancess type is already attached to the type of AMI i choose, so the instances type expected to have is t2 micro.
![Launch EC2 Instances 3](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/Launching%20EC2%20instances%203.gif)
# Keypairs
keypairs created by me. my own key pair containing my name.
![KP](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/KP%20.gif)
# Network setting, Subnets and Auto-assign public IP
I choose VPC lita_project, and subnets: lita_project-subnet-public1 to go with the inbound rules and outbound rules. when assigning public IP it will be on diable, it was enable by me to match with the subnnets and VPC.
![VPC, SUBNET AND ENABLE](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/VPC%2C%20SUBNET%20and%20ENABLE.gif)
# Security group and configure storage
Since the security group has already been created by me all i just did was to select my own security group and configure setting is 8 gp2
![Attaching security group with ec2](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/Attaching%20security%20group%20with%20ec2.gif)
# Instances launch successfully
![ Launch Instances successfully](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/Instances%20launch%20successfully.gif)
# Connect instances
After launching instances showing successful, i clicking on the instances and click on connect, took me to the site that will help configure my instance by clicking on SSH client.
![connect instances](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/Connect%20to%20instances.gif)
# GITBASH
To help me run the following command and to install Apache 
Going to the downloaded keypairs on my download file clicking on it, it show the git bash terminal command: pasting the keypairs after copied my ssh examples which contains my keypairs and ec2 instances and paste it on gitbash, asking do i want to continue YES/NO? YES. It changes from download to "EC2 USERS@ip, after that i run the following commands to install APACHE.
sudo yum install httpd -y, 
sudo systemctl start httpd, 
sudo systemctl enable httpd,
![Gitbash2](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/git%20bash%20step%202.gif)
![Gitbash3](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/git%20bash%20step%203.gif)
![run text 2](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/run%20text%202.gif)
# Apache 
After connecting and runng my command on gitbash, i went back to my instance and copy the link, i paste it on another web to be sure in have successfully connect and run my Apache web text. which came out successful.
![ Apache text](https://github.com/Haabee-theArik1/AWS-Web-Application-Project/blob/main/Text%20Apache%20.gif)
# AWS SERVICVES USE
The AWS services used are : VPC ( Virtual private cloud) use for creating platform for users, SUBNET: logical subdivision of an ip network known as "internet protocol" for connectivity, SG ( Security Group ) this refer to virtual firewall that controls the traffic that allow inbound rule and outbound rule and EC2 Instances (Elastic Compute Cloud) this nis a web based services that allow that allow businness to launch application program.
