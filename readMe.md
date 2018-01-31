# my_aws_journey

I am pretty intrigued by the cloud and everything it has to offer, so as a software developer I decided it should prove to be beneficial to learn AWS (Amazon Web Services).  When I first decided to learn it, I was not aware that there was an actual certification out there; however, I researched more into it and determined that I was not only going to learn AWS – I was going to set a goal to become an Amazon Web Services Certified Developer - Associate.  This is my notes into learning AWS and becoming certified.

I am starting my journey to becoming a Certified Amazon Web Services Developer Associate by using a Cloud Guru course I purchased through Udemy (on sale!).  For those who are unfamiliar, Udemy is a website that has online courses in pretty much, well anything.  The course I am taking is titled “A Cloud Guru AWS Certified Developer – Associate”.  The things that I am looking forward to most in this course are – the databases (got to love yourself some db’s), being exposed to python and php, learning Lambda and building an Alexa skill!  I am also just excited to learn everything and gain a deeper understanding of AWS!

### my_aws_journey_01

A quick history lesson: The inception of AWS was in 2003.  Since then it has evolved and in 2017 there were over 1300+ updates and announcements to the services.  That’s a lot and a lot to keep track of!

AWS is currently the cloud leader with Microsoft Azure and Google behind them.  Oracle, Alibaba and IBM are up and comers to the race!

In 2018 AWS will have 22 regions and 61 availability zones.  Regions?  Availability Zones?  A region is a geographical location that has at least two availability zones.  An availability zone is a data center.  The availability zones are these discrete data centers with their own power, networking and connectivity.  They are geographically isolated, so random disasters in one area do not affect the other availability zone or zones in that region.

Edge locations are endpoints for AWS which are used for caching content.  They typically consists of CloudFront, Amazon's content delivery network (CDN).  My understanding of this – is say there is a popular product at an online store – the information for this product will be held closer to the location that keeps looking at it, so it doesn’t take as long to load.

A list of the current services (from Cloud Guru) and definitions. Services are broken down into categories

Compute
EC2 - elastic compute cloud (cloud compute).  Virtual machines inside of AWS platform.  
EC2 Container Service - run and manage docket containers at scale.
Elastic Beanstalk - for developers who do not understand AWS and want to upload their code.  It will provision things.  All developers have to focus on is their code.
Lambda - code that you upload to the cloud and control when it executes.  You do not have to worry about underlying virtual machines.  Example - if you have a MEAN website where people upload images and overlay text on it - will trigger the overlay once you upload the picture.  
Lightsail - Virtual Private Service - don't really want to understand anything about AWS.  Provisions you with server and fixed ip address.  Has a management console where you can manage the server.  Watered down version of compute or EC2
AWS Batch - batch computing in the cloud
 
Storage
S3 - Simple Storage Service.  Object based storage.  You have buckets and you upload your files into buckets in the cloud.
EFS - Elastic File System - network attached storage.  Mount to multiple virtual machines
Glacier - data archival.  Archive data that you don't need, but want to store for cheap.
Snowball - bring large amounts of data into AWS data center.  Bringing in terrabytes - physically write to a disk and then send it in.
Storage Gateway - virtual appliances/machines that you install in your data center and they replicate information back to S3.  4 different types of storage gateway
 
Databases 
RDS - relationship database service - mysql, postgresql, amazon version of mysql - Aurora, oracle, any relational database
DynamoDB - non relational database 
Elasticache - caching commonly queried things from your database service - example a store and top 10 products
RedShift - data warehousing or business intelligence. Complex queries.  Query has a lot of joins and might take a lot of time.  Built for data warehousing.  Data warehousing Service
 
Migration
AWS Migration Hub - tracking service that allows you to track your applications as you migrate them to AWS.  Visualize your migration
Application Discovery Service - Automated set of tools that detects applications and dependencies.  Way of tracking dependencies for your application.
Database Migration Service - way to migrate your database from on premise into AWS.  
Server Migration Service - helps you migrate your physical and virtual servers up into the AWS cloud.
Snowball - between storage and migration - migrating large amounts of data
 




Networking and Content Delivery 
VPC - Virtual Private Cloud.  Virtual data center.  Configure firewall, availability zone, network address, network acl, root table.  In order to pass any associate exam must know VPC - fundamental important part
CloudFront - content delivery network.  Media assets, video, image files --> cloudfront can store things closer to your user at an edge location
Route53 - DNS service (think of it as an old school telephone book) - results in an IP address
API Gateway - way of creating your own API for your other services to talk to
Direct Connect - running a dedicated line from your corporate head office into Amazon and connect to VPC.
 
Developer Tools 
CodeStar - way of getting group of developers working together easily.  Project Manager tool. Collaborate with other developers
CodeCommit - place to store your code.  Source control service.  
CodeBuild - once you have your code ready - it will compile, run tests against and produce software packages ready to deploy.
CodeDeploy - deploys code
CodePipelien - continous delivery service
X-Ray - debug and analyze serverless application
Cloud9 - IDE environment - develop your code inside AWS console.  Integrated Development Environment.  Acquisition - and released in 2017.
 
Management Tools
CloudWatch - monitoring service
CloudFormation - way of scripting infrastructures.  Turning your infrastructure into code.
CloudTrail - every time you click inside the AWS management console and do something - triggers an API call and CloudTrail logs it.  Stores record for one week.  If you ever get hacked/bitcoin mining - figure out how/where they were using the service.
Config - monitors the configuration of the entire AWS platform.  Visualize your AWS environment.
OpsWorks - similar to elastic beanstalk but more robust.  Uses chef and puppet.  
Service Catalog - manage catalog of IT services.  Anything from virtual machine images to individual operating systems.  Catalog service used by big organziations for compliance.
Systems Manager - interface for managing AWS resources.  Security patch maintenance.  Group resources.
Trusted Advisor - gives advice over multiple disciplines.  Security if ports are left open, if not using services as much as you can.  Sort of like an accountant or an advisor giving you advice
Managed Services - if you don't want to worry about EC2 instances or scaling - managed services can help you out.
 

Media Services
Elastic Transcoder - takes video and resizes so it will look good on different devices
MediaConvert - file based video transcoding service 
MediaLive - broadcast grade high quality video stream - for television, smart phones
MediaPackage - prepares and protects videos for over the internet
MediaStore - storage service optimized for media
MediaTailor - targeted advertising into video streams without sacrificing broadcast quality level of service
 
Machine Learning
SageMaker - easy for developers to use deep learning when coding for their environment - new in 2017
Comprehend - whether or not people are saying good/bad things about your product
DeepLens - artificially aware camera.  Camera can figure out what it is looking at.  You can create an app that can detect someone coming to your front door, if you recognize and if door should open.  Hardware you can buy
Lex - powers Amazon Alexa service.  Way of communication with customers.
Machine Learning - data set into AWS course.  Analyzes and determines an outcome.  Amazon uses it for the recommended products - based on others looking at items…
Polly - not in exam, but we will use it in the course.  Takes text and turns it into speech.  Not old school robot.  Sounds human.  You can choose different languages, regions etc.  We will use to take notes.  Polly will convert to mp3 and then can listen on the go and stream to Alexa.  
Rekognition - video and images.  Upload a file and it will tell you what is in the file. If it is a dog on the beach playing with the ball - it will say dog, beach, ball.  Tells you what it recognizes.
Amazon Translate - translate English into other languages
Amazon Transcribe - transcribes closed caption.  Transcribe brand new service - automatic speech recognition.  Upload videos or mp3's and turns into text.  Can take that and then run it into amazon translate - and then Polly if you want!
 
Analytics
Athena - run sql queries against things in your S3 bucket.  Design a SQL query that will go through and look in all of your buckets.  
EMR - elastic mat reduce - used to process large amounts of data.  Whole bucnh of different servers and chops your data up to be analyzed
CloudSearch - search services
ElasticSearchService - search service
Kinesis - ingesting large amounts of data into AWS.  Such as social media feeds or tweets.
Kinesis Video Streams - reinvent 2018 -ingest large amounts of video
QuickSight - Amazon's business intelligent tool.  From 2016.  fraction of the cost of other business intelligence tools.  1/10th the cost
Data Pipeline - way of moving your data between different AWS services.  In developer associate!
AWS Glue - new service.  Used for ETL extract, transform, load - if data isn't in format you want - Glue is a service that helps you achieve this
  
Security & Identity & Compliance
IAM - Identity Access Management - very first service you use.  Need to know inside out
Cognito - device authentication - authenticate using mobile app such as facebook, gmail - then you can use cognito service to request temporary access to AWS.  Authentication service that gives temporary access to AWS for mobile services
GuardDuty - monitors for malicious activity against AWS 
Inspector - install on virtual machines and EC2 instances - run a bunch of tests - such as security instances.  Generates report and gives you severity list of vulnerabilities.
Macie - scan S3 buckets for PII and alert you
Certificate Manager - SSL Certificates for free if using AWS and registering domains through root53 - manage ssl certificates
CloudHSM - hardware security module - store keys in bits of hardware - per hour billing - hands on security experience
Directory Service - integrating your Microsoft active directory service with AWS service
WAF - web application firewall - layer seven firewall.  Stops sql injections.  Looking at application layer - what is user doing- is this malicious?
Shield - get it by default for cloudfront, load balances, prevent dedoff attacks?  Advance Shield gives you dedicated dedost attack?
Artifact - new service audit and compliance.  On demand access to download AWS compliance reports.  Service Organization Control, Payment Card Industry Reports
 
Mobile Services
Mobile Hub - management console - mobile app create AWS services for you.  Generates cloud configuration file.
Pinpoint - new service way of using targeted push notifications to drive mobile engagement.  Example near restaurant and you have groupon style app - 50% off this restaurant in the next 2 hours.
AWS AppSync - 2017 automatically updates data in web and mobile apps in real time.
Device Farm - way of testing apps on real live devices 
Mobile Analytics - analytic service for mobile
 
AR/VR
Code name Sumerian - used for augmented reality, virtual reality and 3d application design.
Can build 3d rooms - don't really need to know how to code.
Check out book called Ready Player 1
 
Application Integration
Step Functions - manage different Lambda functions and steps to go through
Amazon MQ - message queus (similar to rabbit queues)
SNS - Notification service
SQS - oldest service - decuppling your infrastructure.  If someone uploads image to your MEAN and they tell you what text to overlay - goes to queue - EC2 pulls down and creates image and then removes from queue.  If EC2 dies and does not work right - goes back to the queue.
SWF - simple workflow service - used in warehouses.  Anytime you order package - creates simple workflow job - someone goes and finds, package, postage label and mark as delivery.  
 
Customer Engagement
Connect - contact center as a service.  Like your own call service in the call.  Dynamic, personal, natural customer engagement
Simple Email Service - sending large amounts of email.  Scalable, cost effective, pay as you go
 
Business Productivity
Alexa for Business - dial into meeting room, inform IT printer is broken, reorder ink for printer
Chime - google hangout, zoom meeting, video conferencing
Work Docs - like dropbox for AWS.  Safely and securely store work related documents
WorkMail - like 365 - using email through amazon - like google mail
 
Desktop and App Streaming
Workspaces - running operating system inside cloud and streaming down to your device
AppStream 2.0 - streaming application - running in cloud, but streaming live to your device - similar to what citrix has
 
Internet of Things - iOT one of hottest fields in tech
iOT - thousands of millions of devices sending back information
iOT Device Management - managing at scale
Amazon FreeRTOS - operating system for your micro controllers 
Greengrass - software that allows you to run local compute messaging data caching and machine learning capabilities in a secure way.
 
Game Development
GameLift - service to help you develop games in AWS cloud.


### my_aws_journey_02

Identity Access Management (IAM) is all about setting up users and granting access to the console.  Essentially you are managing your users (teams, positions, etc) and granting them access to specific things in the AWS console for your organization.

With IAM you get – control of your AWS account (root), shared AWS access, granular permissions, way to link to social media accounts (Facebook, google), MFA (multi-factor authentication), temporary access to users or devices when they need to access the services (a storage bucket for example), password restoration policy, integrates with other AWS services, supports PCI DSS compliance.

IAM terms to know:
•	Users – what you think it is – the end users (the employees)
•	Groups - a collection of users under one set of permissions (finance group, HR group, etc) - applying one or more sets of permissions to that group
•	Roles - you create roles and can then assign them to AWS resources (might have an EC2 instance and give it a role to access S3)
•	Policies - a document that defines one (or more permissions) - you attach policies to users, groups and roles - policies is basically permissions.  They can all share the same policy document

An example of creating a role in AWS would be – if you wanted your user to be able to write files to S3 (which is a storage bucket).  You would select the role type EC2.  Select the use case of allowing EC2 instances to call AWS services on your behalf.  Then set the permissions to be AmazonS3FullAccess.  Role Name and type might be S3-admin and the description could be full access to s3 for ec2. You can then apply the role to an EC2 instance.  EC2 instances (virtual machines) and S3 will talk to one another.

my_aws_journey_03

Security Token Services (STS)

Security token services grants users limited and temporary access to AWS resources.  The users are coming from an active directory or federation, federation with mobile app or cross account access.  Federation is joining a list of users in one domain such as IAM with a list in another such as Facebook.  A list of users from one service and a list from another service.  

Identity Store – active directory, Google, Facebook

Identities – users of the services, end users

### my_aws_journey_04

So far I have learned:

IAM consists of:  users, groups (a way to group our users and apply policies to them collectively), roles, policy documents.

Policy Documents – are made up of JSON 

IAM does not apply to regions yet.  Does not matter where you set it up.
 
The root account is simply the account created when first setup your AWS account.  It has complete Admin access – like the super user
  
New Users are assigned an ACCESS KEY ID and SECRET ACCESS KEYS when first created.  These are not a password and cannot be used to login to the console.  You can use it to access AWS via the APIS and command line though.
  
Always setup Multifactor Authentication on your root account – 2 step authentication
 
You can customize your own password policies.

### my_aws_journey_05

EC2 is a webservice that provides resizable compute capacity.  You can boot new server instances in minutes – scaling capacity up and down as requirements change.  They are virtual machines in the cloud, such as linux servers, etc.  Prior to the cloud – you could wait for a server to arrive for weeks, but now you can do it instantly.

EC2 is the main cornerstone of the cloud.

Multiple EC2 options

•	On Demand - allow you to pay a fixed rate by the hour (or by the second) with no commitment. 
•	Reserved – you get a capacity reservation.  Significant discount from the hourly rate.  1 year or 3 year terms.  Good if you know amount of traffic you get
•	Spot - enable you to bid whatever price you want for instance capacity, providing for even greater savings if your applications have flexible start and end times.
o	If spot price is higher than bid price - nothing happens
o	If spot price is lower - provisions your EC2 instances
•	Dedicated Hosts - Physical EC2 server dedicated for your use.  Dedicated hosts can help you reduce costs by allowing you to user your existing server-bound software licenses.  Government likes this
When would I want On Demand?
	-Low cost, flexibility, no up front payment or contract/long term commitment
	-App being developed or tested on AWS EC2 for first time
	-Short-term, or unpredictable workloads

When would I want Reserved?
	-Steady/Predictable use
	-Need a certain amount of capacity
-Scheduled RI’s (reserved instances) available to launch within a time window.  Allows you to match to a recurring schedule

   When would I want Spot Use?
	-Flexible times
	-big data processing at 3:00am
	-urgent computing for large amounts of capacity

When would I want Dedicated Host?
	-regulations don’t allow multi-tenant
	-can be on-demand (hourly)
	-can be reservation 

Instance Types:

D - Density
R - RAM
M - main choice for general purposes apps
C - Compute
G - Graphics
I - IOPS
F - FPGA - field programmable gate arrays
T - cheap general purposes (think T2 Micro)
P - Graphics (think Pics)
X - Extreme Memory

### my_aws_journey_06

Launching my first EC2 instance!.  Turns out it is much easier than I thought it would be.

Step 1.  Login to AWS console
Step 2.  Got to services and choose EC2
Step 3.  Go to launch instance  You will see a variety of virtual machines you can provision and boot up.  Select which one you require.
Step 4.  Click T2 micro and then next.
Step 5.  Configuration details  how many instances do you want?  Under tenancy is where you can configure dedicated host, etc, VPC is a virtual private cloud or data center.  Subnet – which availability zone.  Turn enable termination protection on – this means that you can’t accidentally terminate an instance – you will have to type the name of the instance that you want to terminate in.  In advanced details – this is where you can put text that tells AWS to get certain things – for example:  php.
Step 6.  Add storage.  Requests volume type which is a virtual hard disk in the cloud. 

Things to note with EC2:
- By default – termination protection is turned off – you must turn it on.
- the root ebs volume is deleted upon termination of ec2 instance
- elastic beanstalk root volumes of ami cannot be protected
-Additional volumes can be encrypted.


### my_aws_journey_07

Security groups are virtual firewalls controlling traffic to EC2 instances.  You can have multiple security groups.  You cannot deny traffic – you can only allow it in.  By default it is blocked.

Security groups:
-All inbound traffic is blocked by default - you have to go in and allow
-All Outbound traffic is allowed by default
-Changes to Security Groups take effect immediately
-You can have any number of EC2 instances within a security group.
-You can have multiple security groups attached to EC2 instances.
-Security Groups are Stateful
-If you create an inbound rule allowing traffic in, that traffic is automatically allowed back out again.
-You cannot block specific ip addresses using security groups, instead use network access control lists.
-You can specify allow rules, but not deny rules

### my_aws_journey_08

Elastic File System
 
Amazon elastic file system (Amazon EFS) is a file storage service for Amazon Elastic Compute Cloud (Amazon EC2) instances.  Amazon EFS is easy to use and provides a simple interface that allows you to create and configure file systems quickly and easily.  With Amazon EFS, storage capacity is elastic, growing and shrinking automatically as you add and remove files, so your applications have the storage they need, when they need it.  
 
EFS Features
-Supports the Network File System version 4(NFSv3) protocol
-You only pay for the storage you use (no pre-provisioning required)
-Can scale up to the petabytes
-Can support thousands of concurrent NFS connections
-Data is stored across multiple AZ's within a region
-Read After Write Consistency

EFS is block based storage - instead of object based so you can share with multiple EC2 instances.

With EFS - you can have one file system mounted across multiple servers all serving the same code from the same file system.

### my_aws_journey_09

Installed PHP software development kit for AWS through composer.

Started by downloading a bootstrap script from the cloud guru.  

Started an EC2 instance with amazon linux and T2 micro
S3 admin access role

Used an existing security group.  SSH'd into the instance with my existing key pair and connected to the AWS linux AMI server.

Elevated my privileges to super user

Used composer to install the AWS SDK for PHP.


With the PHP SDK able to interact with S3 buckets.

With PHP there is a program already written where able to pull file down and read what is in it with the software developer kit.  

### my_aws_journey_10

Accessing the public ip address of an EC2 instance.

You can get the public ip address of an EC2 instance while logged into it.  Need to know the url to access metadata

Ssh into the ec2 isntance and elevate to root

Curl http://169.254.169.254/latest/meta-data/public-ipv4

After that it gives you the public ip address --> you are looking ofr meta data not user data

### my_aws_journey_11

Elastic load balancers are virtual pliance that spread the load of traffic across servers.  There are 2 types - application load balances and class balances.

Application load balances are new and they operate at layer 7 by checking the application.  They are the preferred according to Amazon

Classic load balances operate at layer 4

In EC2 you go to load balances.  

Routing Decisions
	-MyClassicELB (name it)
		-external load balancer because we want web traffic
		-choose what ports listening to
		-choose existing security group
	-Configure Health Check --> the guts of load balancer
	-Advanced:
		-Response timeout -->amount of time it waits for a response
		-Interval --> how long waits between response
		-Unhealthy threshold --> how many times it needs to fail health check before determined EC2 is unhealthy
		-Healthy threshold --> opposite --> how many times an unhealthy instance needs to pass to be determined healthy.
	-Add Tags -->elastic load balances will cost money if you leave it on.  Product ELB Value ON

AWS gives a DNS name, not an ip address
You can simulate an unhealthy ec2 by deleting a file

Go to DNS --> straight to html
-AWS always uses DNS for ELB --> so you have ec2 instances behind your DNS so nothing goes down

1 subnet equals 1 availability zone

Target Groups are used for routing in application load balances

Instances monitored by ELB are reported as Inservice (healthy) or OutofService (unhealthy)

Health Checks check the instance health by talking it to --> they look for a file such as index.html

Own DNS name --> never given an IP

### my_aws_journey_12

The available SDK's (Software Developer Kits):
-Android, iOS, JavaScript (Browser)
-Java
-.Net
-Node.js
-PHP
-Python
-Ruby
-Go
-C++

These are the languages supported by Amazon.

SDK Default Regions --> Always US-EAST-1
Some have default regions such as Java, Node.js does not

### my_aws_journey_13

EC2 Launches in 2006

Data Centre --> took 10 days to get the server

2006 Amazon launched EC2 which allowed you to provision servers from an API call.  You did not have to provision individual servers.  Basically infrastructure for code.  Infrastructure as a service --> still have to manage windows, linux, etc.  Infrastructure as a service only goes so far.  Platform as a service --> elastic beanstalk.  You can upload your code and amazon would create the web service for you.  Amazon would handle it for you, but you are still managing your operating service.  Containers --> Docker.  They are isolated and lightweight, but you still have to deploy to your server and keep them running.

Lambda released in 2015.  You do not have to manage infrastructure, platforms, containers.  Amazon takes care of it.  You take your code and upload it.  You take an event trigger which will call your lambda function.

What is Lambda?
-Your data center
-Hardware
-Assembly Code/Protocols
-High Level Languages
-Operating Systems
-Application Layer/AWS APIs
-AWS Lambda

Amazon's definition:  AWS Lambda is a compute service where you can upload your code and create a Lambda function.  AWS Lambda takes care of provisioning and managing the servers that you use to run your code.  You don't have to worry about operating systems, patching, scaling, etc.  You can use Lambda in the following ways:
	-As an event-driven compute service where Lambda runs your code in response to events.  These events could be changes to data, an Amazon S3 bucket or an Amazon DynamoDB table.
	-As a compute services to run your code in responses to http requests using Amazon API Gateway/API calls made using SDK

Lambda --> React to a particular event or trigger.  The user uploads a picture to S3 which triggers a Lambda function --> which takes it and stores it in S3 which then in turn triggers a Lambda event and return file back to user.  Which can trigger another Lambda event and stores it in another S3 bucket

Each instance - every time you do something with Lambda --> that is one instance.  If you have multiple users --> multiple instances.  Lambda scales automatically.  You do not have to worry about elastic load balance.  Lambda scales out automatically (adds elastic load balances instances).  

Different types of Lambda triggers:
	AWS Console:
		-Services - Compute - Lambda
	
	Triggers:
		API Gateway
		AWS iOT
		Cloudwatch Events
		Cloudwatch Logs
		CodeCommit
		Cognito Sync Trigger
		DynamoDB
		Kinesis 
		S3
		SNS
		Alexa Skills Kit
		Alexa Smart Home
		CloudFront
	
Using API Gateway:
	-User browsing in google chrome --> send http request to get a new webpage --> triggers Lambda function and returns response to user.  Scales out automatically so if 2 users with 2 http requests --> scales out and invokes 2 Lambda functions
	-Multiple lambda functions responding to multiple requests
	
Very different than EC2 instances as you might only have 2 instances --> those 2 instances/servers will be what responds to all requests.

What Languages are supported by Lambda?
	-Node.js
	-Java
	-Python
	-C#

How is Lambda Priced?
-Based on the number of requests.  First 1 million requests are free --> after that .20 per 1 million requests thereafter.  You are literally paying only when someone is using your application

-Duration --> calculated from time code begins executing until it returns/terminates --> rounded to the nearest 100ms.  Price depends on amount of memory you allocate to your function.  Function cannot execute over 5 minutes.

Lambda
	-NO SERVERS!
	-Continuous Scaling - instantly!
	-CHEAP!   
	
Practical use:  Every time you speak to Alexa --> Lambda function and it is Lambda speaking back to you.

REMEMBER:
Lambda scales out (not up) automatically
Lambda functions are independent.  1 event = 1 function
Lambda is serverless
S3, API Gateway, DynamoDB, LAMBDA are serverless services
Lambda functions can trigger another Lambda function
Architectures can be complicated.  Debugging can be difficult!  That is why you have the x-ray service which debugs
Can use Lambda to back up s3 buckets to other s3 buckets
Lambda triggers -->
	API Gateway
	AWS iOT
	Cloudwatch Events
	Cloudwatch Logs
	CodeCommit
	Cognito Sync Trigger
	DynamoDB
	Kinesis 
	S3
	SNS
	Alexa Skills Kit
	Alexa Smart Home
	CloudFront
Lambda execute time is 5 minutes
Lambda languages - Node.js, Java, Python, C#