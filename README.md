# Create automation in AWS environment.


### Pre requisites
      1. Ansible Installed 
      2. AWS Cli API 
      3. Account in AWS

![alt text](https://i.imgur.com/Z1JsPna.png)

### SETUP

   ###### Resources created by script ansible in playbook.yml

      - Launch instance 
      - Create security group
      - Add public_ip
      - Enable SSH service 
      - Attach disk EBS in instance
      - Install packpages

   ###### Setup ansible-role-install-docker in main.yml

      - Update your O.S 
      - Format disk ext4 default
      - create directory for shared volume
      - mount device 
      - add permision for jenkins 

   ###### Setup docker.yml 

      - install packpages
      - add key 
      - install docker and compose
      - install docker-python modules

   ###### Setup jenkins

      - Deploy jenkins in container 
      - Install java
      
  For execute without formating disk use 
  `ansible-playbook -i ip/filehosts, -u usuario --private-key chave --skip-tags empty playbook.yml`

---



