# SRE_Cloud_Computing_AWS
## User Journey
### Cloud computing with AWS
##### AWS Services 

- Creating github repo to push the markdown doc
- Amazon Web Services (AWS)

## SRE (Site Reliablity Engineer) Role:
- Reduce toil(tedious or repetitive tasks) and ensuring that the underlying infrastucture is running smoothly. Maintaining systems and tools so that they are working as expected. On top of this they're responsible for monitoring critical applications and services to minimise downtime.  

## Benefits of cloud computing:

# Ease of use
- Users are able to quickly and securely host their applications.
- You can use AWS Management Console or APIs to access AWS's application hosting platform.

# Fexibilty 
- Able to select any of the different services you require.
- Receive a virtual environment used to load the software and services for your application.
- Easy to migrate

# Robustness
- If one region goes down the Auto Scaler can redirect to another Availability Zone (AZ)
- Can scale up and down on demand

# Cost effective
- Pay for resources which are in use.
- Pay as you go format

## What is AWS?
- Amazon web services(AWS) is used for hosting cloud services. Big organisaitons and companies usch as Netflix and the Home office use aws to host their services. It provides servers,storage, networking, remote computign, emial , mobile development and security . 

## AWS Global Infrastructure 
- The AWS Global Cloud is the most secure,extensive and reliable cloud platform that provides you the cloud infrastructure where and when you need it with a single-digit milisecond latency.

## Regions VS Availability Zones
- Availability Zones are multiple, isolated locations within each Region.
- Each Amazon EC2 Region is designed to be isolated from the other Amazon EC2 Regions. This achieves the greatest possible fault tolerance and stability.

## The Four Pillars of Cloud Computing
- Performance
- Security 
- Reliability
- Functionality

## CDN - Content Delivery Network
- A content delivery network (CDN) refers to a geographically distributed group of servers which work together to provide fast delivery of Internet content. A CDN allows for the quick transfer of assets needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos


## ON-PREM vs HYBRID
- Hybrid cloud refers to a mix of on-prem storage, private cloud services and public cloud services such as AWS.

## ON-PREM vs PUBLIC CLOUD
On-prem is more secure and reliable but reliant on physical maintenance
Public cloud removes responsibility and pressure of maintenance, it is also easily scalable.

## Connection between local host and public cloud (AWS)
Requires permissions through roles, ports and keys
# Local Host
local machine, desktop pc, laptop
Stores file.pem (in .ssh folder) to access public cloud
# Public Cloud
- AWS
- Needs to be secure
-- Creates aws file.pem as SSH key
-- Important, key is not shared with non-authorised parties
- We need to create a virtual machine on the cloud - ec2 (elastic compute service)
-- Virtual machine similar to hardware - requires specific components!
AWS Diagram
[image](https://user-images.githubusercontent.com/48529086/159467057-83f5029f-cc2e-40dd-9aaa-b86a52ebdf87.png)
- Creating of an EC2 Instance
- Login and access to AWS services
- Choose AMI (ubuntu 18.0.4)
- Choose EC2 Instance Types (default bc cheap lol)
- Configure Instance Details
- Subnet choose "default a"
- Add storage
- Tag instance (for me it's 105_sre_jack_{purpose})
- Configure security groups
- SSH on My Ip (port 22)
- HTTP on anywhere (port 80)
- HTTPS ONLY if you have ssl certificate
-Review instances
- Select key name
Launch :D
___________________
## In a terminal window (preferably gitbash) follow steps from AWS:

- The link should look like this:

- ssh -i /path/my-key-pair.pem my-instance-user-name@my-instance-public-dns-name

- Once connected update all the required services via sudo apt-get update -y and sudo apt-get upgrade -y commands. Then install via sudo apt-get install {name} -y

- Example: after installing nginx with a sudo apt-get install nginx -y command your output from the website should look like this: picture

