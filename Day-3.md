# The Assignment

-  Create and delete ninja directory on host machine
    - Status: [hosts](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/hosts.png)
    - Learning: In inventory we can manage organized goup of hosts.
-  Set hostname on all nodes from remote machine
    - Status: [hostname](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/hostname.png)
    - Learning: using command module we can perform shell operation on hosts, and learned about the concept of hostname & its configuration as well (/etc/hosts , /etc/hostname).
-  Fetch os of all nodes and store o/p into a file, use min two different machine of different flavour of os.
   - Status: [issue_os](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/issue_os.png) issue in copying output in a folder.
   - Learning: Using command module, and got to know about the location where os information lies. Usage of redirect operator.
-  Add three group into hosts file through ansible module.
      - Debian ( ip of debian machine)
    - Centos ( ip of centos machine)
    -  All ( ip of all nodes )
- Status : [hosts](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/hosts.png)
- Learning: In inventory we can manage organized goup of hosts.

# Problem statement: Using Adhoc command

Step 1:

- Install apache on Debian machine
- Cross check apache isntalled or not from remote machine
- Apache runn  on 8082 port
- Create two virtual host
- Restart apache from remote machine  

  - Status- Debian machine is not available(technical issue) 


Step2:

- Install nginx on centos machine
  - Status: [nginx_install](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/nginx_install.png)
  - Learning: Usage of yum module to manage package on nodes.
-  Nginx run on 8080 port.
   - Status: [8080_port](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/8080port1.png) , [restartnginx](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/restartnginx.png)
   - Learning: configuration of nginx manually via editing nginx.config (/etc/nginx/nginx.config), using lineinfile module to edit the content of a file on remote servers .


Step3:

- Configure Nginx - configure it to run as reverse proxy to apache
  - Status: [tomcat_install](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/tocat_install.png) , Pending
  - Learning: Learned about the concept of reverse proxy and forward proxy, and their configuration manually. But facing some issues using Ansible, hence it is pending.
