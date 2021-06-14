# AWS-Workspaces  

https://d1.awsstatic.com/Projects/provision-cloud-desktops/Provision%20Desktops%20in%20the%20Cloud%20-%20Implementation%20Guide.pdf  

\\\  Steps to build workspaces
1) Create Elastic IP address
2) Create VPC=10.0.0.0/16 with VPC wizard  
3) Create subnets
   - Public subnet 10.0.1.0/24
   - Private subnet #1 10.0.2.0/24 (Different AZ)  
   - Private subnet #2 10.0.3.0/24 (Different AZ)  
4) Create Route-Table
   - Main Route-table associates with public subnet to Internet GW (IGW)
   - Another Route-table associates with private subnets to NAT GW
5) Create NAT GW
6) Create Directory 
7) Create Workspaces 
   - Install required softwares
   - Create image
   - Create bundle for each user

https://user-images.githubusercontent.com/16419246/121849020-0b265180-cd15-11eb-8b2f-9355b6719481.jpg
![workspaces](https://user-images.githubusercontent.com/16419246/121849252-517bb080-cd15-11eb-85c9-2c8c98d014b5.jpg)

\\\
