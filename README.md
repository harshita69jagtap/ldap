######################################### Openldap implementation using Ansible Playbook###############################

Points to remember when running playbooks:-
- openldapserver.yaml runs on a target which has python 2.7 as default as installed pip and MySql-python package
  are compatible with this version
- Kindly pay attention to the entries to be entered in /etc/hosts files of target machines ,they are hardcoded 
  ip addresses from a NAT Network of cidr 10.0.2.0/24
- The user on ansible server will be the same user that will run the playbooks on respective targets with granted
  sudo privileges without entering password
- When running both the playbooks kindly manually add the user on remote hosts to wheel/sudo group and edit the
  sudoers file so that the sudo user can run the playbook without entering the password
 
