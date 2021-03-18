# ABOUT THE EXECUTION OF YAML FILES

## You are supposed to run these playbooks in specified order.


### 1. ec2_final.yml
  - This playbook will launche 3 instances over AWS CLOUD.
 
 
### 2. master_final.yml
  - This playbook will configure k8s masternode. 


### 3. worker_final.yml
  - This playbook will configure k8s workernodes and will join the above cluster.
        
### 4. mtapp_final.yml
  - This playbook will configure Multi-tier setup.This will launch a  pod with wordpress application and connect it to another pod containing mysql database.

Example Playbook Execution Command
----------------
      ansible-playbook <playbook_name.yml>

