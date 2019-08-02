# ansible-ec2-server

- Ansible Playbook for provisioning CentOS 7 AWS EC2 servers.

## Before Install

- Update Environment Variables.
```
export AWS_ACCESS_KEY_ID=<Access Key ID>
export AWS_SECRET_ACCESS_KEY=< Secret Access Key>
```

- Update the the variables in vars/main.yml.
```
vi vars/main.yml
```

   - Run the playbook
```
ansible-playbook ec2_provision.yml
```

   - Connect to Instance.
```
$ ssh -i <YOUR_SSH_KEY>.pem centos@<INSTANCE_PUBLIC_IP>
```
