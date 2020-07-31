# ec2-creation-ansible-playbook

- This is the simplest script for creating EC2 instance using ansible

## Install Ansible 
### Requirement
AWS cli
```
curl "https://s3.amazonaws.com/aws-cli/awscli-bundle.zip" -o "awscli-bundle.zip"
```
```
unzip awscli-bundle.zip
```
```
sudo ./awscli-bundle/install -i /usr/local/aws -b /usr/local/bin/aws
```

Boto
```
pip install boto boto3 botocore
```
### Installation
To install ansible you have to install pip first
```
sudo yum install python-pip
```


After that you can install ansible usung

```
sudo pip install ansible
```

After the installation of ansible you have to follow the follwing steps:
  - Create a new folder(Wherever you want).
  - Now in that folder create a  ```yml``` file in that folder (File with ```.yml``` extension).
  - And creat the ```hosts```file(```Note``` that ```hosts``` dose not have any extension).

Now, you have created the ```yml``` file, the next step is open the terminal and fire the command 
```
ansible-playbook -i hosts aws_ec2_docker-jenkins.yml --connection=local
```
or
```
ansible-playbook -i hosts aws_ec2_docker-jenkins.yml --connection=local -vvv 
```
```Note :-``` "```-vvv```" is used to see detail logs 
