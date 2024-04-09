# Convert-AWS-EBS-Volume-from-gp2-to-gp3
Using AWS CloudWatch and Lambda, we automate resource management by triggering Lambda functions upon Amazon EBS volume creation. Leveraging CloudWatch Events, we monitor GP2 EBS volumes, seamlessly converting them to GP3 for enhanced performance.

# Step-by-step implementation 
step 1:- Create an lambda function as ‘ebs_volume_check’ and runtime as ‘python 3.10’ also we Create a new role with basic Lambda permissions.

