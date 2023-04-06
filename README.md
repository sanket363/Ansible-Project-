# Ansible-Project

## To Create the Ansible Project which hosts the webserver on the two of its Nodes follow below steps

### Step 1

Create 3 AWS EC2 machines with Ubuntu OS and with Same Key pair

For creating AWS EC2 machines follow [this](https://docs.aws.amazon.com/efs/latest/ug/gs-step-one-create-ec2-resources.html) documentation. Its recommended to create EC2 machine of the image Ubuntu

(Note: To establish connectivity between three remote machines, it is not necessary to have an AWS account. Instead, any three remote machines can be used as long as they are configured to share keys, allowing them to establish a connection with each other.)

### Step 2

Installing Ansible on the Ubuntu Machine
