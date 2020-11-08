# Ansiblepythonscript
Ansible playbook to bring up a new EC2

### 1.Install Ansible's prerequisites
sudo apt install python3
sudo apt install python-pip
pip3 install boto 
pip3 install boto3
sudo apt install ansible

### 2.Create SSH keys to connect to the EC2 instance 
ssh-keygen -t rsa -b 4096 -f ~/.ssh/my_aws

### 3.Create Ansible Directory(Optional)
mkdir -p AWS_Ansible/group_vars/all/
cd AWS_Ansible
touch playbook.yml

### 4.Create pass.yml
Provide access Credentials

### 5.Create playbook.yml
 Ansible playbook to bring up a new EC2 instance
 
### 6.Create list_instances.py
 All pre-requisites to run the Python script.
 
### 7.Executing Ansible to Create instances
ansible-playbook playbook.yml
#### Create the instance
ansible-playbook playbook.yml --tags create_ec2
#### Get the public DNS
ansible-playbook playbook.yml
### 8.Run python code
python3 list_instances.py
