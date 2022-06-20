# My First Cloudformation Stack

High available WordPress setup on AWS, based on the AWS "WordPress_Multi_AZ" template:

- added EFS filesystem, to share the DocRoot between the webservers
- edited the bash scripts to mount EFS and install WordPress
- added SNS topic, to notify the autoscaling changes
- added Security Groups for EFS and public URL access

![WordPress-Designer](https://user-images.githubusercontent.com/10097753/174570511-c4b22ce2-1e54-47d6-a980-c6458d46047c.png)
