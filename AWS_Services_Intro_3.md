# AWS Service Introduction -  Part 3

## SERVICES - Security, Identity & Compilance


## AWS IAM 
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

## Certificate Manager


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

## Step Function
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


