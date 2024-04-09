# Convert-AWS-EBS-Volume-from-gp2-to-gp3
Using AWS CloudWatch and Lambda, we automate resource management by triggering Lambda functions upon Amazon EBS volume creation. Leveraging CloudWatch Events, we monitor GP2 EBS volumes, seamlessly converting them to GP3 for enhanced performance.

# Step-by-step implementation 
step 1:- Create an lambda function as ‘ebs_volume_check’ and runtime as ‘python 3.10’ also we Create a new role with basic Lambda permissions.

![1 xXybsYaFcpPaQf301waZag-1](https://github.com/jagati2/Convert-AWS-EBS-Volume-from-gp2-to-gp3/assets/105737471/55068ea3-70e6-45ed-a491-a39c2439d592)

after creating an lambda function just test it so we confirm that lamda fuction is work correctly.

![1 nC26nWkyUfrOqUZAB7KfYw](https://github.com/jagati2/Convert-AWS-EBS-Volume-from-gp2-to-gp3/assets/105737471/2d57a2e2-0138-4aca-9f13-8a212444af29)

![1 fSxINxPdSnQ7PsKXyFfBtw](https://github.com/jagati2/Convert-AWS-EBS-Volume-from-gp2-to-gp3/assets/105737471/76353031-0b39-4d27-93a3-620a4f1609fe)

step 2 :- Go to cloudwatch service then go to event section and create an role for the ebs volume creation. Select service name as ec2 , Event type is EBS Volume Notification ,specific event is createVolume. In target section we select existing lambda fuction and configure details.

![1 RQHwVid29ZbpwkFQpEEHmQ](https://github.com/jagati2/Convert-AWS-EBS-Volume-from-gp2-to-gp3/assets/105737471/1b626a74-3a70-494f-9cd0-2d496decf8ff)

give name as per your requirement and creating role.

![1 uwyW7w0ST8r4LdEsuVJLRg](https://github.com/jagati2/Convert-AWS-EBS-Volume-from-gp2-to-gp3/assets/105737471/cfdc18a0-e387-4b8d-8437-8bbc826c1bb9)


