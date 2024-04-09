# Convert-AWS-EBS-Volume-from-gp2-to-gp3
Using AWS CloudWatch and Lambda, we automate resource management by triggering Lambda functions upon Amazon EBS volume creation. Leveraging CloudWatch Events, we monitor GP2 EBS volumes, seamlessly converting them to GP3 for enhanced performance.

# Step-by-step implementation 
step 1:- Create an lambda function as ‘ebs_volume_check’ and runtime as ‘python 3.10’ also we Create a new role with basic Lambda permissions.

![1 xXybsYaFcpPaQf301waZag-1](https://github.com/jagati2/Convert-AWS-EBS-Volume-from-gp2-to-gp3/assets/105737471/55068ea3-70e6-45ed-a491-a39c2439d592)
