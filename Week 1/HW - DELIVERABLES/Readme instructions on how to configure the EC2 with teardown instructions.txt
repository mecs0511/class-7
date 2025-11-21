Creating EC2 Instance 

1. Click on Security groups on the left side 

2. Click on create security group 

Basic details 

Security group name,  description

VPC use default option 

Inbound rules 

Click Add rule 

HTTP Source (anywhere IPv4)

SSH  Source (anywhere IPv4)

Outbound rules leave it as it is

Tags are optional 

Click on create security group 

Check your Inbound rules and Outbound rules 


On the left side click on instances 

Click on launch Instances either button works 

Name and tags

Name 

Skip application and os images 

Instance type 

t3.micro

Create key pair ( use defaults)

Click on create key pair 

Network settings 

Select existing security group

Common security groups choose one from the drop down menu 

User data 

Put script in the all the way at bottom of the screen into the user data box

Click launch Instance


Copy Public DNS 

use http://paste in public dns and hit enter


Check Instance box and click connect 

Check everything under the EC2 INSTANCE CONNECT then click connect for the black screen 


You use ping 8.8.8.8 control z to stop



Create a template


A template is used to automate the creation of new instances.


Left side go to Instances 

Go to actions, image and templates, create template from Instance

Create lauch template 

Lauch template name and description 

Name the template 

Template version description 

You can skip to Resource tags and add tags

Advanced details should have your script 

Click on create launch template 

Launch Instance from template

Click on view launch templates 


Launch Instance

Teardown Instructions

Console Home

EC2

Under EC2 go to dashboard

Under resources Instances(running) should be zero (0)

If you have instances running, click on Instances(running)

Check the box for the instance listed

Look under instance state, click on terminate (delete) instance

Check your regions foe instances running in other regions

Your instance page should after you refresh the page there should not be any instances running
