# CloudWatch_Alarm_Publish_To_SQS.yaml-cloudFormation
### Description: 
  #### 'AWS CloudFormation Sample Template SNS_Publish_To_SQS:
  Sample template showing how to grant rights so that you can publish SNS notifications
  to an SQS queue. Note that you will need to specify the CAPABILITY_IAM flag when
  you create the stack to allow this template to execute. You can do this through
  the AWS management console by clicking on the check box acknowledging that you understand
  this template creates IAM resources or by specifying the CAPABILITY_IAM flag to
  the cfn-create-stack command line tool or CreateStack API call. **WARNING** This
  template creates an Amazon SQS queue and an Amazon SNS topic. You will be billed
  for the AWS resources used if you create a stack from this template.'
  
### STEPS:
#### 1) Upload CloudWatchlogsWithSNS.Yaml
#### 2) Upload instances.yaml 
#### 3) Upload sns.yaml 
  

~~~
Upload CloudWatchlogsWithSNS.yaml File.
~~~

**Description:**
Upload this file in aws-cloudformation. This Stack create Enviroment for Ec2 Instance. It create Vpc with 1 subnet, which having internet access. It also create Outputs of some resources which we use later. 



### Tips:
#### 1.
~~~
Use Public IPs of EC2 Instances to test data. 
~~~
  
