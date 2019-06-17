# CloudWatch_Alarm_Publish_To_SQS.yaml-cloudFormation
When alarm trigger it will pass message to the SQS through SNS. 
### Description: 'AWS CloudFormation Sample Template SNS_Publish_To_SQS:
  Sample template showing how to grant rights so that you can publish SNS notifications
  to an SQS queue. Note that you will need to specify the CAPABILITY_IAM flag when
  you create the stack to allow this template to execute. You can do this through
  the AWS management console by clicking on the check box acknowledging that you understand
  this template creates IAM resources or by specifying the CAPABILITY_IAM flag to
  the cfn-create-stack command line tool or CreateStack API call. **WARNING** This
  template creates an Amazon SQS queue and an Amazon SNS topic. You will be billed
  for the AWS resources used if you create a stack from this template.'
  
### STEPS:
#### 1) 
  
  
### Upload Stack:
~~~
Upload EC2WithRds.yaml File.
~~~

**Description:**
Upload this file in aws-cloudformation. Stack Created by this file will Create two EC2 Instances with Ubuntu AMI, and Relation Database Service (RDS) with their Read Replica and MultiAZ unable. First Instance is connected to main RDS Instance and second one is connected to Read Replica of that RDS Instance just for Read operation from database. Then this stack create Redis Elastic Cache and attach it to the Second Instance that have Read Only access to the data base. Simple Database Web Application is already on S3 bucket that have publically accessable.    




### Tips:
#### 1.
~~~
Use Public IPs of EC2 Instances to test data. 
~~~
  
