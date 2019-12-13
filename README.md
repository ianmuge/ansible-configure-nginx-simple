# Deployment Instructions
On CLI you can run the command as shown below substituting the user.pem for own aws generated pem and playbook with actual playbook name.
```
ansible-playbook  -u ec2-user  -i ec2.py  -T 60 -f 100 --private-key=~/{{user}}.pem  -l {{hosts_identifier}} BaseConfig.yml
```