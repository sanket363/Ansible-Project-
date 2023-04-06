# Ansible-Project

## To Create the Ansible Project which hosts the webserver on the two of its Nodes follow below steps

### Step 1

Create 3 AWS EC2 machines with Ubuntu OS and with Same Key pair

For creating AWS EC2 machines follow [this](https://docs.aws.amazon.com/efs/latest/ug/gs-step-one-create-ec2-resources.html) documentation. Its recommended to create EC2 machine of the image Ubuntu

(Note: To establish connectivity between three remote machines, it is not necessary to have an AWS account. Instead, any three remote machines can be used as long as they are configured to share keys, allowing them to establish a connection with each other.)

### Step 2

Installing Ansible on the one of the 3 Ubuntu Machine. For ansible installation click [here](https://github.com/sanket363/Ansible-Project-/blob/main/steps-to-install-ansible.md)

### Step 3

copy the private key from local to Host server (Ansible_host) at (/home/ubuntu/.ssh)

### Step 4

Access the inventory file using 
```bash
sudo vim /etc/ansible/hosts
```

Now in the /etc/ansible/hosts file we will need to insert the pubic ip address of the other 2 EC2 machines with creating the Group for it scroll to the last line of the file and copy paste below

```bash
[servers]
<public-ip1> ansible_ssh_private_key_file=/.ssh/<privateKey-pair-Name>
<public-ip2> ansible_ssh_private_key_file=/.ssh/<privateKey-pair-Name>
```
### Step 5

Creating a playbook to install Nginx create the file with any name with the extension .yml
For the ansible playbook click [here](https://github.com/sanket363/Ansible-Project-/blob/main/playbook.yml)

### Final Step

deploying a sample webpage using the ansible playbook for this run below command. Be aware to be in the same path where your playbook is situated

```bash
anisble-playbook playbook-name.yml
```

