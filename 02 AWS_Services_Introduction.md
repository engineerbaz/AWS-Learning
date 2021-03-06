# **AWS Service Introduction**
------------------------------------
Total 165+ services covering Compute, Networking, Security, business application, IoT and etc
- Compute 
- Storage 
- Network
- Database 
- migration & transfer
- Analytics
- Special (IoT/ML/AI)

[AWS Documentation ](https://docs.aws.amazon.com/index.html)

# COMPUTE

## EC2:
- Pure Compute Service based on RAM & CPU
- ElasticCompute Cloud EC2
- Could be on Windows or Linux
- On-demand, spot
- Per hour & Per second based pricing

## LightSail
- VPS Server
- Both LS & EC2 are compute service but the difference is 
  - Complete package (including CPU, RAM. HDD, networking )
  - No scaling in LS
  - LS is only public
  - Monthly charges

- VPS server on an hourly basis with complete package (CPU, RAM, HDD, data OUT service) 
- LS is fixed-configuration and no communication in between to LSs

## ECR 
- Elastic Container Registry
- Store and manage Docker Images for containers 


## ECS 
- Elastic Container Service 
- Service where images run to make containers like Docker

## EKS 
- Elastic Kubernetes Service 
- Allows to run Kubernetes on AWS
- For orchestration of containers like Kubernetes 

## Lambda
- Serverless architecture 
- Can run any code without provisioning /managing server 
- Pay only for compute when it is scheduled ( no need to run  server every day)

## Batch
- Enables to run hundreds of computing jobs on AWS 
- Free service , just need to pay only EC2 resource

## Elastic BeanStalk
- Deploying web application (build pack ) on Ruby/Java/PHP/NodeJS/Go & Docker to AWS, it will deploy using Apache/Nginx/IIS
- Free service 

## Serverless application Repository
- Managed Repository for Serverless application
- Allows to find, deploy, publish, share, store & assemble serverless architecture

--------

# STORAGE

## AWS S3 
- Simple Storage service (S3)
- Object Storage service
- Google cloud Storage In Google , OSS in Alibaba
- Virtually unlimited. 
- Max. PUT size is 5GB
- Object can be uploaded of max 5TB 
- Works on Linux & Windows both
- 99.999999999% durability

## EFS 
- Elastic File System 
- works on Linux 
- Like NFS
- Elastic means  can grow up and down
- Connect using IP of DNS name

Object = dynamic </br>
Block = Fixed like HDD

## FSx
- FsX = for Windows 
- It needs Active Directory 
- two types
  - Windows File server
    - Native windows FS
  - Lustre
    - Optimized for compute-intensive workload

EFS uses EXT4 </br>
FSX uses SMB in window 

## S3 Glacier
- Glacier like archive for long time 
- 9.999999999 % durability
- Police record, medical &  financial record. 
- Cheap service 

## Storage Gateway
- hybrid storage service that enables On Prem application to seamlessly use AWS Cloud = 
- Need VPN
  
Cache based = main data in cloud and cache on-prem </br>
Volume-based. =  data of branch to move to HQ

## Backup 
- To schedule backup of any service 
- Easy to centralize and automate the backup of data across AWS services & on-Prem


--------------

# DATABASE

## RDS 
- Relational Database Service
- Makes it easy to setup, Operate & Scale a relational DB in cloud
- suite of DB
- DB Server can run 6 types of DB
  - Arora 
    - AWS propertiship
  - Postgre SQL, MYSQL, MariaDB
    - Community based (They are OpenSource but needs to pay for machine/compute) 
  - Oracle & Microsft 
    - License & Compute Charges also 

- Oracle license (per month charges )
 - EE Enterprise (6 months free )
 - SE = Standard Edition

- Microsoft license 
  - Express &  Web --  Free
  - Standard & Enterprise -- charged

## DynamicDB 
- No SQL query like MangoDB
- Fast & Flexible, Low latency
- DynamoDB can handle more than 10 trillion requests per day and can support peaks of more than 20 million requests per second.

## ElastiCache
- Redis and Memcached (Open Sourced, server cost is charged)
- Popular for Gaming, FinTech, IoT

## Neptune
- Fast reliable graph Database
- Core of Neptune is for HP graph DB , can store billions of relationships and queries in msec latency

## RedShift
- Amazon Redshift is a fast, fully managed, petabyte-scale data warehouse 
- Like Data warehouse 

## QLDB 
- Quantum Ledger DB
- Fully Managed Ledger Database
- Transparent, Immutable & Cryptographically verifiable transaction log
- Fully managed (managed by AWS)


## Document DB
- MongDB compatible DB
- Fast, reliable, Fully managed

Lab for RDS & DynamicDB

--------------
# Migration & transfer

## Migration Hub
- A single location to track progress of application migration across multipleAWS & Partnar solutions
- Alos provide Key metrics and progress

## Application Discovery Service
- helps Enterprise customers to plan migration by gathering information about on-prem DC

## Database migration Service
- Helps you to migrate DB to AWS quickly & securely

## Server Migration Service
- SMS is an agentless service makes it easier and faster to migrate thousnad of on-prem workload to AWS

## AWS Transfer for SFTP

- Fully managed service enables to transfer files over SFTP (Secure FTP), into & out of Amazon S3
- SFTP is also known as SSH FTP (Secure Shell)
- used to exchange workflow across different industries (FinTech, Health, retails)

## Snowball
- petabyte-scale data transport solution that uses apploances to transfer large amount in/out to cloud

## DataSync
- Data transfer service that simplifies, automates, accelerates moving & replicating data bw on-prem storage & AWS Storage over internet or AWS DirectConnect
- It remobves the need to modify applications, Develop screipt or manage Infrastructure

---------

-----------------

# NETWORK & CONTENT DELIVERY 

Network services Works on Layer 2 /3 and 4 </br>
Content delivery = sharing caching data 

- VPC = Virtual Private Cloud 
- Network of Router, Switches, Firewall 
- VPN, NAT Gateway

All Nodes (Routers, Switch etc) are virtual as they are not physical
</br>
Can a VPC consist of multiple region VMs? No

## VPC
- Virtual Private Cloud
- Logically isolated section in AWS Cloud, resource can be launched
- both IPv4 and IPv6 can work

## Cloud Front
- Content delivery Network
- It is like CDN Cache Data Network 
- Clone of your data can be placed in different location where your user location so low latency and fast

## Route 53
- 53 port number 
- DNS based service 
- Domain Name ,DNS record, Zones
- effectively connects user requests to infrastructure running in AWS – such as Amazon EC2 instances, Elastic Load Balancing load balancers, or Amazon S3 buckets 
- and can also be used to route users to infrastructure outside of AWS

## API GW
- create/publish/maintain/monitor APIs 
- API = Application Programmable In

## Direct Connect 
- The connection between your location and AWS 
- Dedicated fiber line
- Till 10Gbps speed, Where VPN is around 300mbps (or depends on speed you have)

We can use any other DNS services than route 53, can we?  YES but no routing functionality 

## APP mesh
- For application level networking
- E2E visibility of microservices for high availability

## Cloud Map 
- Discovery service of  all your running services 

## Global Accelerator
- Network Layer service direct traffic to optimal end points 
- Improves availability

---------------------

# DEVELOPER TOOLs

## Code Star 
- Develop/build & deploy  apps on AWS 
- Dashboard for all software development

Code Star & BeanStalk slightly overlaps ?
</br>
Code Star is like to VS Code 
At Beanstalk is a real location where the app is deployed ( can be deployed in Docker, lambda function 
Supports JS, Ruby, Python PHP

## Code Commit
- Source Control Service Like GIthub, Gtlab, Bitbucket

## Code Build
- Compiles code and run test & produce software
- Dry run (unit testing)

## CodeDeploy
- Automates software deployment to EC2, Lambda or on-prem
- helps in avoiding downtime during updates /rollout

## Code PipeLine
- Its continuous integration and continuous integration for application and infrastructure update

## Code Cloud9
- Its IDE (Integrated Development Environment) like Eclipse, visual code, atom & sublime

## X-Ray
- Analyze, debug and troubleshooting

debug for coding
trouble for infra issues  

--------------------

# DEVELOPER TOOLs

## Code Star 
- Develop/build & deploy  apps on AWS 

Code Star & BeanStalk slightly overlaps ?
</br>
Code Star is like to VS Code 
At Beanstalk is a real location where the app is deployed ( can be deployed in Docker, lambda function 
Supports JS, Ruby, Python PHP

## Code Commit
- Source Control Service Like GIthub, Gtlab, Bitbucket

## Code Build
- Compiles code and run test & produce software
- Dry run (unit testing)

## Code Deploy
- Automates software deployment to EC2, Lambda or on-prem

## Code PipeLine
- Its continuous integration and continuous integration for update

## Code Cloud9
- Its IDE (Integrated Development Environment) like Eclipse, visual code, atom & sublime

## X-Ray
- For analysis, debug and troubleshooting

debug for coding
trouble for infra issues  

--------------------

# MANAGEMENT & GOVERNANCE
 
## AWS Organization 
- Account management system 
- For consolidated billing and control of multiple accounts

## Cloud Watch 
- Monitoring service and alert as well
- Can work for EC2 instances, DynamicDB Table, RDS DB instances or custom materics

## Auto Scaling 
- Horizontal scaling 
- Adjust capacities to maintain performance in lowest cost
- 

## Cloud Formation 
- A Common Language to describe & provision all infrastructurein  Cloud network (that is used for future reference ) 
- Infra aaS
- YAML, JASON can be used.
- Deployment manager in GCP, Resource Manager in Azure 
- Terraform can make any resource

Programing for App development 
Coding for Infrastructure

## Cloud Trail 
- Audit logs for compliance 
- Operational & Risk auditing

## AWS Config 
- For enabling assess audit and evaluate configuration 

## OpsWork
- Its a Configuration Management 
- use code to automate the configurations of your servers.
- Ansible, 
- Allow automated Config management
- Chef & Puppet = opswork

## Service Catalog
- Create catalog IT services
- including everything (images, server, SW, HW, DB)

## System Manager 
- Gives visibility and control AWS infrastructure
- For getting Inventory management 
- Help in getting access in VMs Using SDK (without Putty)

## Truster Advisor 
- For suggestion to reduce cost, increase service performance
- real time guidance

## Managed Service 
- service for automating infra management task 
- for large Enterprises in migration

## Control Tower 
- To set up a secure account
- best practices

## License Manager 
- For license migration
- BYOL = Bring Your Own Li

## WA Tool
- Well Architecture Tool
- throughout product cycle 
- For suggesting best practices

## Health Dashboard
- NMS of regions
- Dashboard for health of AWS services 

## Chatbot
- To automate answer queries using SLACK

----------------


## MEDIA SERVICES
Normally related to broadcasting channels like News channels

## Elastic Transcoder
- Used for media transcoding (conversion of media) of files for making it compatible to play on smartphones,PCs & Tablets

## Kinesis video stream
- Realtime 
- Securely stream video from connected devices to AWS for analytics, ML 

## Media Connect (Elemental)
- Connect different media 
- Distribute inside and outside the cloud
- Elemental is suite of services 

## Media Convert (Elemental)
- Its a file-based video transcoding service 
- broadcast-grade
- create video on demand (VOD)

## Media Live (Elemental)
- Broadast-grade live video 
- Delivery to Broadast TV & internet-Connected
- multiscreen devices like TBs, Tablets

## Media Package (Elemental)
- Prepares & protect video for delivery over the internet-Connected multiscreen

## Media Store (Elemental)
- Storage service for optimizing media for performace
- Low latency required to deliver live streaming video Content
- Not an Storage devices!

## Media Tailor
- Tailoring /insert adds/advertisement in videos
- Targeted audience 

## Elemental Appliances & Software 
- Powerful media encoder which can take input from HDI-SDI , IP over ethernet or local files and produce ,multiple video output 
- Web browser via HTML
- Web services ReST interfaces

---------
## MACHINE LEARNING 

## SageMaker
- Fully-maanged to enable data sciientest to build, train & deploy machine learning models
  
## Comprehend
- National Language processing (NLP) uses ML to find insights & relationships in text
  
## DeepLens
- Its an harware
- Fully programmable video camera 
- Helps put deep learning 
- programmable 
- Worlds 1st wireless deep learning enabled video camera

## Lex
- conversational interface using voice & text
- advanced deep learning
- ASR (Automatic Speech Recognition) for converting speech to text & National Language understanding (NLU)

## Machine Learning
- AWS working for 20 years
- Generic ML service

## Polly 
- Convert text to speech
- Language, accent, male or female will be asked

## Rekognition
- provide pictorial / video analysis for objects

## Tanscribe
- automatic speech recognization (ASR)
- speech to text conversion by using API

## Tranlate
- Tranlate is a neural machine tranlation
- can be used after Transcribe (converts text to speech) then translate it other Language

## Personlize
- Personlize ML
  
## Forecast
- Using previous record 
- Time series forcasting
- useful in retail, financial planning, supply chain, 

## Textract
- text Recognition in documents 
- Analysis of your application

## DeepRacer
- learning system for learn reinforcement 
- automomus driver less 
---------

# ANALYTICS

## Athena
- interactiv query service for analyze data in S3 
- Severless (no infrastructure to manage only pay for the queries you run)

## EMR
- data platform for processing vast amounts of data using open source tools such as Apache Spark
- Map reduce

## CloudSearch
- To set up , manage & scale a search solution
- Its works on app

## Elasticsearch Service
- log analytics for infra O&M
 
## Kinesis
- Securing media stream 
- Analyze as well

## Quick sight
- Like Power BI 
- Quick insights for your data 

## Data Pipeline
- move data between AWS Services (Compute, Storage )
- Also on-prem data sources at specified intervals

## Glue
- extract, transform & load client to prepare & load data for analytics

## Lake Formation
- Setup secure data lake in days 
- centralized repo 

## MSK 
- Managed Streaming for Apache Kafka
- bild , run 
- applications that use Apache Kafka to process Stream
- Apache Kafka is OpenSource for Realtime streaming data PipeLine
- 



----


One Question
Difference between Storages Block Volume, object based & File

block is fixed amount of st
Obj is like Gdrive  

block is like HDD
Obj is like Gdrive  

===============
# AWS Service Introduction -  Part 3

## SERVICES - Security, Identity & Compilance


# AWS IAM 
- Enables you to Securely control access to AWS services and resources for your user
- Using IAM, can create & Manage AWS users & group & use permissions to allow & deny 

## RAM 
- resource Access Manager 
- Enables you to easily & securely share AWS resources with any AWS account or within organization
- Share AWS Transit GW, subnets configurtaion and Route 53 , 
****

## Cognito
- Lets add user sign up/in & access control to you web or mobile app


## Secret Manager
- Makes it easier to manage Secret (database cred, pwd,3rd party API Key)
- Can store & control access to these secret centrally 

## Guard Duty
- Manage threat detection service
- IDS 
- Check account
  
## Inspector 
- Automated Security product
- Check threat VM vulunerability


## Macie
- Security service that uses machine learning to automatically discover , classify & protect sensitive data 


## SSO 
- Single Sign-On (SSO) Makes it easy 

******

# Certificate Manager


## KMS
- Key Management Service
- managed service to create the encryption keys used to encrypt data

## CLoudhsm
- Hardware Security Module
- Hardware based that generate and use own encyption 

KMS > HSM

## Directory Service
- Like Microsoft Active Directory
- Managed service 
- works on windows 7 , server 2012

## WAF & Shield 
- WAF is Web Application Firewall 
- Lets you monitor web requests for Amazon Cloudfront distribution and restrict access to your contecnt
- Shiel is managed DDoS protection service that safeguards web Application running on AWS
- stateful
- 2 stype of Shield 
- shield can be attached to VMs

## Artificat


## Hub
- Like Suite
- single  place that aggregates organizes & prioritize your security

-----

# Mobile service

## Amplify
- CI of Hosting service for modern web application 

## Mobile Hub
- Featuure selection and configurtaion and automatically provisions 

## App Sync
- automatically updates the data in web and mobile application  in realtime and update data for offline users as they reconnect

## Device Farm
- App testing service taht lets you test and interact with android /IoS and web app 

## Mobile Analytics

# AR & VR 
- Augmented Reality
- service
- Virtual Reality 
- 
## Sumerian
Lets you create and run VR & AR and 3D 


-----

# Step Function
- Makes easy to coordinate the component 


## EventBridge
- Serverless event bus service that makes easy to connect your application with data

## MQ 
- Message Queue
- Message broker service for Apache ActiveMQ taht makes it easy to setup

## SNS 
- Simple Notification service
- Via email, sms 
- for security breach, high billing
- cloud watch only generate event

## SQS 
- Simple Queue service
- For queuing service, make it easy to decouple and scale microservices , distribution systems & serverless application

## SWS
- Simple Workflow service 
- Helps developers build, run, and scale background jobs that have parallel or sequential steps


---

# COST Managemnet

## Cost Explorer
- Tool that Enables you to view and analyze your cost and usage

## Budget
- enbles you to plan service usage/Cost and instance reservation 
- how close your budget.

## Marketplace Subscription 
- Its like Google playstore for android
- Like Cisco sell Virtual Firewall
- Two prices involved
  - Owner
  - AWS resoource cost

---

# Customer Engagement

## Amazon Connect 
- CCaS = Contact Center as Service 
- Call Center services 

# Pinpoint 
- makes easy to engage customers by tracking the way in which they interact with Applications
- A targeted push Notification and mobile engagement 
  
## SES 
- Simple Email service
- Cloud based email sending service 
- like SMTP server

---

# Business Applications

## Alexa for businsess 
- Can help people stay organized and focused thing that matter.
- Hardware 

## Chime
- Communication software
- onine meeting 

## Workmail 
- secure business email 
- calendar integrated 
- Desktop and mobile app 

-----
# END USER COMPUTING 

## WorkSpace 
- DaaS = Desktop as a Service 
- can easily provision virtual, Cloud-based microsoft windows Desktop
- Horizan in VM 
- Zen  Desktop in Citrix 
- virtual PC in microsoft*
- Horizan in VMware 

## AppStream 2.0
- only share some or one app to user 
- ZenApp in Citrix
- RemoteApp in microsoft

## Workdocs
- Secure , file collaboration and Managemnet service with extensible SDK

## WorkLink 
- Provides secure to internal website / app from mobile(IoS/android)

----
# IoT
Internet of Things 

## IoT Core 
- secure, bi directional Communication between inter-Connected device 
  - Sensor
  - Actuators
  - Embeded microcontrollers 
  - smart Applications
  - AWS Cloud 
- possible to collect telmetry data form multiple device and store and analyze data
- can create application that Enables your user to control these devices from their phone
  
## FreeRTOS
- Free RealTime OS  that augment FreeRTOS kernel with libraries for connectivity, security, and over-the-air (OTA) updates 
- OpenSource

## 1-Click 
- Makes easier for enterprise customers to incorporate simple IoT devices into their Workflow 
- these devices can securely connect to AWS IoT 
- these device can trigger Lambda function (in Java, Phython, C#)

## Analytics
- Automates step required to analyze data to IoT devices 
- Filters, transforms, and enrich IoT before storing 

## Device Defender 
- Audit configurtaion , monitor connected devices & mitigation of security threat
- enforces consistent security policies across all IoT devices

## Device Management
- A registry that helps to manage things (specific device or logical entity)
- Can be phsical device(bulb, light)

## IoT Evernt 
- monitor or device for failure or change in operation
- continously watches IoT sensor data from devices, processes, application and other AWS services 
- 
## Greengrass
- Extends Cloud capabilities to local devices
- Allows local devices to collect and analyze data closer to source of info
- Greengrass developers can use Lambda function to create Serverless application to local execution

## SiteWise 
- Can collect, organize,search, & consume equipment data form Industrial equipment at scale
- provides Gateway software 
- GW can read data directly from server 

## IoT Things Graph
- Orchestation service simplifies IoT deployment

----

# Game /Robotic/ BlockChain / satellite

## Gamelift 
- Managed Service for deploying, Operating & scaling dedicated game server for session based multi player ganes
  
## RoboMaker
- Robot OS makes it easier for creating robitcs application at scale
- extends the ROS (Robotic OS) framework to cloud

## Managed BlockChain 
- For creating & managing BlockChain Network using Open source framework

## Ground Station
- Enables you to control satellite Communication, 
- dDownlink and process satellite and data 

---
