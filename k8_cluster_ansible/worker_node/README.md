Role Name
=========

### worker_node

Requirements
------------
   - As the execution of master_final.yml get completed, you can directly run this playbook.

Role Variables
--------------
   - Variable in this role is storing join command that will help worker nodes to join the k8 cluster.This command will load dynamically.

Important Note
------------
***It is adviced not to edit the join command.On doing so worker nodes will fail to join the cluster.***

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
