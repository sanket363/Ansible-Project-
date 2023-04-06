# Ansible-Project

## To Create the Ansible Project which hosts the webserver on the two of its Nodes follow below steps

### Step 1

Create 3 AWS EC2 machines with Ubuntu OS and with Same Key pair

1.Sign in to the AWS Management Console.
2.Click on the "Services" dropdown and select "EC2" under the "Compute" category.
3.Click on the "Launch Instance" button.
4.Select the "Ubuntu Server" AMI by scrolling down or searching for it in the search bar.
5.Choose the instance type you want to use for your Ubuntu machines, such as t2.micro.
6.Click on "Next: Configure Instance Details" button.
7.On the "Configure Instance Details" page, select the desired options for your instances, such as network settings, VPC, subnet, etc. and click on the "Next: Add Storage" button.
8.Configure the storage settings and click on the "Next: Add Tags" button.
9.Add any desired tags to your instances and click on the "Next: Configure Security Group" button.
10.On the "Configure Security Group" page, create a new security group and give it a name.
11.Add a rule to allow incoming SSH traffic from your IP address to the security group.
12.Add another rule to allow incoming SSH traffic from the security group to itself.
13.Click on the "Review and Launch" button.
14.On the "Review Instance Launch" page, review your instance settings and click on the "Launch" button.
15.On the "Select an existing key pair or create a new key pair" dialog box, choose "Create a new key pair" from the dropdown menu.
16.Give the key pair a name and click on the "Download Key Pair" button to download the private key file.
17.Click on the "Launch Instances" button to launch your instances.

(Note: To establish connectivity between three remote machines, it is not necessary to have an AWS account. Instead, any three remote machines can be used as long as they are configured to share keys, allowing them to establish a connection with each other.)
