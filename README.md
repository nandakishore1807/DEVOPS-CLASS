DEVOPS--CLASSLINK
- Zoom Link:https://zoom.us/j/96078845638?pwd=dEZzSTBhQUtJNnR3VndtUDVYL1M1Zz09 
- Zoom Credentials: Zoom id: 960 7884 5638
- Passcode: devops
----------------------------------------------------------------------------------------------------
**DAY-1 (18-01-2022)
- VIDEO LINK:https://www.youtube.com/watch?v=d3u72SxI7ZE&t=445s
- TOPICS DISCUSSED ON 18/01/2022
  - DEVOPS INTRODUCTION

--------------------------------------------------------------------------------------------------
**DAY-2 (19-01-2022)
- VIDEO LINK:https:https://www.youtube.com/watch?v=n4tlrIbEbPs
- TOPICS DISCUSSED ON 19/01/2022
  - LINUX COMMANDS DISCUSSED

----------------------------------------------------------------------------------------------------
**DAY-3 (20-01-2022)
- VIDEO LINK:https:https://www.youtube.com/watch?v=xN1I4MTWbZo
- TOPICS DISCUSSED ON 20/01/2022
  - LINUX COMMANDS DISCUSSED

-----------------------------------------------------------------------------------------------------
**DAY-4 (21-01-2022)
- VIDEO LINK:https:https://www.youtube.com/watch?v=vN3JCmrT9GA
- TOPICS DISCUSSED ON 21/01/2022
  - DEVOPS TOOLS
    - AWS
    - GITHUB
    - DOCKER
    - ANSIBLE
    - KUBERNETES
    - MAVEN
    - JENKINS
    - SPLUNK
  - AWS ACCOUNT CREATION
  - DEMO OF EC2(SERVER LAUNCH)

-----------------------------------------------------------------------------------------------------
**DAY-5 (24-01-2022)
- VIDEO LINK:https://www.youtube.com/watch?v=zho0BsWVU6M
- TOPICS DISCUSSED ON 24/01/2022:
  - EC2(SERVER LAUNCH)
  - SECURITY GROUPS

------------------------------------------------------------------------------------------------------
**DAY-6 (25-01-2022)
- VIDEO LINK:https://www.youtube.com/watch?v=qRrpPEus0go&t=2933s
- TOPICS DISCUSSED ON 25/0/2022:
  - IAM(IDENTITY ACCESS MANAGEMENT)
  - MFA(MULTI FACTOR AUTHANTICATION)
    - DASHBOARD
    - USER--CREATE USER
    - ROLES--CREATE RULES(HOW MANY SERVICES ARE YOU NEED)
    - POLICES--CREATE POLICES(SERVER ACCESSABILITY TIME EXAMPLE:SOMETIMES SERVER ACCESSABILITY INCREASED AND SOMETIME LOW)
    - IDENTITY PRIVIDER

-----------------------------------------------------------------------------------------------------
**DAY-7 (27-01-2022)
- VIDEO LINK:https://www.youtube.com/watch?v=ZuI3sB7FUho
- TOPICS DISCUSSED ON 27/01/2022
  - S3BUCKET(SIMPLE STORAGE SERVICE)
  - IT IS STORE THE FILES RANGE(0-5GB)
  - UPLOADING FILE IN S3BUCKET AND ACCESS 

------------------------------------------------------------------------------------------------------
**DAY-8 (28/0/2022)
- VIDEO LINK:https://youtu.be/klHKLSLHObI
- TOPICS DISCUSSED ON 28/01/2022
  - S3 BUCKET
  - LOAD BALANCING
  - CREATING VPC(VIRTUAL PRIVATE CLOUD):
    - IP ADDRESSES
    - SUBNETS
    - ROUTING
    - INTERNET GATEWAY

------------------------------------------------------------------------------------------------------
**DAY-9 (29-01-2022)
- VIDEO LINK:https://youtu.be/vuSYOf9-_dM
- Topics discussed on 29/1/2022:
  - VPC Creation
  - Subnet Creation
  - Routing Table Creation
  - Attaching the same to internet gateway
  - discussed about Public DNA
  - discussed about Public VPC
  - Deleting the created VPC

**step by step launch ec2 by using created vpc
  
- step-1

openvpc
---------
yourvpcs
----------
create vpc--vpcname--ipv4-10.0.0.0/16-create vpc--actions-editdnshostname--enable--save changes

- step-2

subnets
-------
create subnet--given already created vpc id--subnet name--any one select availability zone--ipv4-10.0.0.0/16--create subnet

- step-3

internet gateway
-----------------
create internet gateway--name--create internet gateway--actions--attach to vpc--given already created vpc id--give ok

- step-4

route table
-------------
alredy one route table alredy created--select the name--routes--edit routes--add route--0.0.0.0/0--select internet gateway--select the alredy created gate way--save changes
select sunnet associate--select edit subnet associate--select given one--ok

- step-5
open ec2
------------
launche instance--select any one of ami--select t2 micro free trair--choose instance type---select the alredy create vpc-to launch the ec2--open git bash to connection--now ec2 is launched by using created vpc
without any error.

------------------------------------------------------------------------------------------------------------------------------
**DAY-10 (31-01-2022)
- VIDEO LINK:https://youtu.be/EFZzknfFXsg
- Topics discussed on 31/1/2022:




-------------------------------------------------------------------------------------------------------------------------------
**DAY-11 (01-02-2022)
- VIDEO LINK:https://youtu.be/HaQvaEP2SJ8
- TOPICS DISCUSSED ON 01/02/2022:
- NATGATE WAY

- Load Balancing--
- Auto Scaling--High Availability

- Elastic Load Balancer(ELB)
  - microservices                             
    - /user                       
    - /app                       
    - /user-name
  - target group 
    - customized apps
    - (nginx)(apache)
  - round robin mechanism
    - Request--Response

           EFS(Elastic File System)

### Network Load Balancer is a Faster Then Application Load Balancer

**NETWORK LOAD BALANCER
- NLB IS WORKS ON TCP/UDP PROTOCOL
- OSI LAYER
- PORT BASED ROUTING

**APPLICATION LOAD BALANCER:
- ALB------HTTP/HTTPS
- APPLICATION LAYER
- PATH BASED ROUTING

---------------------------------------------------------------------------------------------------------------------------------
**DAY-12 (02-02-2022)
- VIDEO LINK:https://www.youtube.com/watch?v=eA0N_elaO7I
- TOPICS DISCUSSED ON 02/02/2022

- first we launch the EC2 Instances

- load balancing
    - Load Balancers             
    - Target Groups

- STEP-1:-
                                - FIRST WE CREATING TARGET GROUPS:-

   - CREATE TARGET GROUPS FOLLOW THE APPICATION LOAD BALANCER PROTOCOL(HTTP/HTTPS)
   - SELECT TARGET GROUPS-CREATE TARGET GROUPS--GIVE THE TARGET NAME AND SELECT APPLICATION LOAD BALANCER PROTOCOL--AND SELECT TO REGISTER TARGETS INSTANCES--INCLUDE AS PENDING      BELOW--CREATE TARGET GROUP
 
   - CREATE TARGET GROUPS FOLLOW THE NETWORK LOAD BALANCER PROTOCOL(TCP/UDP/TLS)
   - SELECT TARGET GROUPS-CREATE TARGET GROUPS--GIVE THE TARGET NAME AND SELECT NETWORK LOAD BALANCER PROTOCOL--AND SELECT TO REGISTER TARGETS INSTANCES--INCLUDE AS PENDING          BELOW--CREATE TARGET GROUP

- STEP-2:-
                                        - LOAD BALANCERS:-
  - ALB CREATION:-
    - SELECT CREATE LOAD BALANCER--SELECT APPLICATION LOAD BALANCER--GIVE THE LOAD BALANCER NAME AND SELECT THE ALP TARGET GROUP--CREATE LOAD BALANCER
  - NLB CREATION:-
    - SELECT CREATE LOAD BALANCER--SELECT NETWORK LOAD BALANCER--GIVE THE LOAD BALANCER NAME AND SELECT THE NLB TARGET GROUP--CREATE LOAD BALANCER

- Auto Scaling
    - Launch Configurations
    - Auto Scaling Groups

- STEP-3:-
                                     - Launch Configurations:-
  
  -- Select the Launch Configurations create Launch Configurations--first we create the launch templates--and give the template name and select AMI(amazon machine image)--and        select any one of security group--create launch template
   - now create Launch Configurations--give name,select any one of AMI and select instance(t2-micro),and select key pair is requried or not--create Launch Configurations

- STEP-4:-
                                      - Auto Scaling Groups:-

  -- Select Auto Scaling Groups--Create Auto Scaling Groups--

  - Step 1:
    - Choose launch template or configuration:-
      -- and give name And Select Switch to Launch configuration And Select A Launch configuration --Next
  - Step 2:
    - Choose instance launch options:-
      -- Select Availabiliy Zones--Next
  - Step 3 (optional)
    - Configure advanced options:-
      -- Select Attach to an existing load balancer--Select Existing load balancer target groups--Select Health check type(ELB)--Next
  - Step 4 (optional)
    - Configure group size and scaling policies:-
      -- Next
  - Step 5 (optional)
    - Add notifications:-
      -- Next
  - Step 6 (optional)
    - Add tags:-
      -- Next
  - Step 7
    - Review:-
      -- Create Auto Scaling Groups
   
 -------------------------------------------------------------------------------------------------------------
 **DAY-13 (03-02-2022)
- VIDEO LINK:https://www.youtube.com/watch?v=FjZyVZJvEg0
- TOPICS DISCUSSED ON 03/02/2022
- Config Group Size & Scaling Polices

- Config Group Size
  - Group Size Optimal
  - Check The Activity--Check The Instances

- Scaling polices
  - none
  - key and value optional
 
- create a dynamic scaling policy
- create a cloud watch
  - select matric--alarm
  
   - static                              
   - greater>=threshold             
   - value-70                                      

   - select ec2 
   - auto scaling group

   -  matric name
   -   cpu  utilization
   -   Auto scaling group

- simple notification service()

------------------------------------------------------------------------------------------------------
 **DAY-14 (04-02-2022)
- VIDEO LINK:https://www.youtube.com/watch?v=FjZyVZJvEg0&t=20s
- TOPICS DISCUSSED ON 04/02/2022
- cloudwatch

-----------------------------------------------------------------------------

**DAY-15 (05-02-2022)
- VIDEO LINK:https:https://www.youtube.com/watch?v=GnhaFyLmJMQ
- TOPICS DISCUSSED ON 05/02/2022
- ec2 server launch using redhat
- ec2 server launch using ubantu

------------------------------------------------------------------------
**DAY-16 (07-02-2022)
- VIDEO LINK:https://youtu.be/GxSXp6Qw7XE
- TOPICS DISCUSSED ON 07/02/2022
- Terraform-Hashicorp
  - steps in Terrafoem
    - configuration file
    - init--plan--apply
- IAC tools
- Docker Ansible,puppet,saltstack,cloudformation

-----------------------------------------------------------------------
**DAY-17 (08-02-2022)
- VIDEO LINK:https://www.youtube.com/watch?v=7AHa_VBeGqk&t=2202s
- TOPICS DISCUSSED ON 08/02/2022
1. first we launch the ubantu server 20.04
2. connect to git bash using ssh key
   - convert to root user: sudo -i
   - update:sudo apt-get update
3. install terraform in ubantu 20.04:-
- Repository Configuration:
  - curl -fsSL https://apt.releases.hashicorp.com/gpg | sudo apt-key add -
  - sudo apt-add-repository "deb [arch=$(dpkg --print-architecture)] https://apt.releases.hashicorp.com $(lsb_release -cs) main"
  - sudo apt install terraform
- Choosing Terraform Versions:
  - apt policy terraform
  - sudo apt install terraform=0.14.0
- check the version:
  - terraform --version
4. terraform to be configured for aws account
   - choose iam accpunt and select the manage access keys--
   - create new access key
- connect to access keys and seceret keys
1. file1 - first we create a file using .tf extension
  - vi provider.tf
  - goto google search aws provider and copy the
   Usage:
  provider "aws" {
  region     = "us-west-2"
  access_key = "my-access-key"
  secret_key = "my-secret-key"
}

2. file2 - and create another file
   - vi main.tf --and search google main.tf 

  resource "aws_instance" "app_server" {
  ami = ""
  instance_type = "t2.micro"
  
  tags = {
    Name = "ExampleAppServerInstance"
  }
}  

5. innatiated the terraform
   - terraform init
6. validate the terraform
   - terraform validate
7. terraform apply
   - terraform apply  
 - now server is launch
8. terminate the server
   - terraform destroy


- Using infrastructure as a code

- overview of launch server using terraform concept:-
  1. terraform install in server
  2. terraform to be configured for aws account
  3. terraform-- provide.tf--region,aws access key,secret key addes
  4. terraform--vi main.tf--ec2--name,ami,t2.nicro,tag
  5. terraform init
  6. terraform validation
  7. terraform apply

- launching the multiple instances using terraform
1. Goto Google search launch multiple instances for aws terraform
2. Goto vi main.tf
resource "aws_instance" "app_server" {
  ami = ""
  instance_type = "t2.micro"
  count=3
  tags = {
    Name = "ExampleAppServerInstance"
  }
}  
3. terraform init
4. terraform validate
5. terraform apply
6. adding security groups
  - goto google search main.tf terraform security group

- :wq!         ----save&quit

---------------------------------------------------------------------------------------------------------
**DAY-18 (09-02-2022)
- VIDEO LINK:https://www.youtube.com/watch?v=XFXYphx8h0k&t=570s
- TOPICS DISCUSSED ON 09/02/2022
- 
