# ec2-launch-server
==============
Ansible Playbook for provisioning CentOS/RHEL AWS EC2 servers.

## Instructions
   - Clone repo, update environment variables and the variables.yml file.
```
git clone https://github.com/rgdevops123/ansible-ec2-server
cd ansible-ec2-server

export AWS_ACCESS_KEY_ID=<Access Key ID>
export AWS_SECRET_ACCESS_KEY=< Secret Access Key>

vi variables.yml
```

   - Run the playbook
```
ansible-playbook ec2_provision.yml
```

   - Copy over your ssh key.

   - Connect to Instance.
```
$ ssh -i <YOUR_SSH_KEY>.pem centos@<INSTANCE_PUBLIC_IP>
```
