Role Name
=========

multi_tier :-this role will setup multi-tier setup on your kuberneters cluster

Requirements
------------
- It is compulsory to edit you Username and Database Name in files > mysql.yml
- Setup database password in file > secret.yml in encoded formate
 ### To encode your password - use command(linux)
      echo 'your_pass' | base64
- By default hostname for database is wordpress-mysql
#### Note:- HOSTNAME AND PASSWORD will help you to access your mysql-database



# Login to mysql database from master node.
   **Run these command over master_node.**
 
    kubectl get pods
    kubectl exec -it <mysql container pod id> -- bash
    
### Login to mysql database using hostname wordpress-mysql and provide database password. 


License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
