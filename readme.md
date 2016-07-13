##AMAZON S3

Data storage, your online drive letter

Different solution needed for running a virtual machine with an application and controllers

This is what your application would use for back-end storage

####Video  
Introduction to S3 [https://aws.amazon.com/s3/](https://aws.amazon.com/s3/)

####Why

Instead of buying racks, backup, hiring staff, doing security

####What is it

Cloud storage

"Simple Storage Service"

secure, durable, scalable

web interface to store and retrieve

for backups and static files

Your own personal Dropbox or Evernote for business

####Details

pay only for storage, not setup or minimum

levels by frequency of access
- Standard
- Standard - IA = infrequent
- Glacier = low-cost, long-term archive
- 
migrates automatically

there are charges and different latency times for accessing these

by itself or with EC2 or with data migration services

encryption of data and for access

AWS Free Tier includes 5GB storage, 20,000 Get Requests, and 2,000 Put Requests with Amazon S3

###Transferring data

direct

stream

ship physical drive

transfer acceleration

####Used by

- Netflix
- AirBnb
- SmugMug
- NASDAQ

#####Netflix
makes instances

hosts microservices

org can move to DevOps as data moves to cloud

- test and experiments on new services or instances
- instead of negotiating with IT for servers

####AirBnb
can focus on primary business, not hosting

#####Compares with Google Cloud Storage and Microsoft Azure

####RESOURCES

Basic docs [https://aws.amazon.com/s3](https://aws.amazon.com/s3)

Google Cloud [https://cloud.google.com/](https://cloud.google.com/)

Microsoft Azure [https://azure.microsoft.com/en-us/services/storage/](https://azure.microsoft.com/en-us/services/storage/)

Good blog post on price compairson [http://www.cloudberrylab.com/blog/amazon-s3-azure-and-google-cloud-prices-compare/](http://www.cloudberrylab.com/blog/amazon-s3-azure-and-google-cloud-prices-compare/)

Calculate estimated storage costs for your data set with price calculators.  See above.


####Using it

[Hosting a Static Website on Amazon S3](http://docs.aws.amazon.com/AmazonS3/latest/dev/website-hosting-custom-domain-walkthrough.html)

[General web hosting info on S3](http://docs.aws.amazon.com/AmazonS3/latest/dev/WebsiteHosting.html)

Set up

- choose location
- make a bucket
- store
- get prior versions

[Log in to Console](https://console.aws.amazon.com/console/home)

- register domains
- set up two buckets - your domain.com, www.yourdomain.com
- upload website files, make public, and configure www... to go to root site.
- Route 53
    - create hosted zone
    - create  two A records (NS and SOA already given), one for root, one for www...

####Interface (use SDKs)

For browser JS, Node JS, Ruby, etc.
[http://aws.amazon.com/code](http://aws.amazon.com/code)

`bower install aws-sdk-js`
