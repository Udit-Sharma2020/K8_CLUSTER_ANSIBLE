Role Name
=========

- Ec2_instance

Requirements
------------

- You should have an IAM user created over your AWS account.Download the AWS credentials as these are important for execution of this role  

Role Variables
--------------
    In vars/main.yml u must provide your AWS-CREDENTIALS.
           aws_access_key: <access_key>
           aws_secret_key: <secret_key>


Security 
------------
    To secure your sensitivedata ie:AWS-credentials , it is adviced to encypt vars/main.yml of this role
     use command:
                    ansible-vault encrypt ec2_instance/vars/main.yml
    
To execute Playbook
----------------

    Including an example of how to use your role (with variables passed in encrypted form):
         Use command:
                    ansible-playbook --ask-vault-password ec2_final.yml


