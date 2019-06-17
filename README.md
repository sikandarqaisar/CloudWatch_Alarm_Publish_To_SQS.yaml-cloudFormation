# CloudWatch_Alarm_Publish_To_SQS.yaml-cloudFormation


<img src= "https://github.com/sikandarqaisar/aws-cloudformation-EC2-with-RDS/blob/master/template.jpg" width="600" height="600">


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



~~~
Upload instances.yaml File.
~~~

**Description:**
This Stack create Ec2 Instance on Public subnet which we created on earlier stack. This Ec2 Instance have cloudWatch agent. So when we upload this stack we also installing cloudWatch agent in it through UserData. 


~~~
Upload sns.yaml File.
~~~

**Description:**
This Stack create three different types of alarm with SNS and SQS. SQS contains QueuePolicy for all Users all permissions. This Stack also creates CloudWatch Event. So by this Stack when alarm trigger it pass message to SQS through SNS. And if any type of changes occours it pass that change to SQS through SNS.
