# My First Cloudformation Stack

High available WordPress setup on AWS, based on the AWS "WordPress_Multi_AZ" template:

- added EFS filesystem, to share the DocRoot between the webservers
- edited the bash scripts to mount EFS and install WordPress
- added SNS topic, to notify the autoscaling changes
- added Security Groups for EFS and public URL access

**Infrastructure details:**
- Application Load Balancer
- Autoscaling Group
- EC2 instances (up to 5)
- EFS filesystem
- RDS Aurora MySQL database Multi-AZ or Single-AZ
- SNS notifications
- OS:
    - AmazonLinux2
    - Apache 2.4
    - PHP 7.3
    - MysQL client 5.7
    - latest Wor

**Cloudformation Designer schema:**
![WordPress-Designer](https://user-images.githubusercontent.com/10097753/174570511-c4b22ce2-1e54-47d6-a980-c6458d46047c.png)

To deploy the infrastructure, upload the json file in Cloudformation and fill the required fields.
The deployment takes approx 25 min.
