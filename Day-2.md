# Topic: Ad-Hoc Commands and Basic Ansible Modules
The Assignment

Perform the following operations using ad-hoc commands and ansible modules :

 1)Fetch and display to STDOUT Ansible facts using the setup module.
- Status:

    2)Fetch and display only the "virtual" subset of facts for each host.
- Status  :  

3)Fetch and display the value of fully qualified domain name (FQDN) of each host from their Ansible facts.
- Status :   

4)Display the uptime of all hosts using the command module.
- Status:  

5)Ping all hosts except the 'control' host using the --limit option
- Status:

6)Setup Java8 on the hosts in the "App" group using the apt module.
- Status:

7)Setup and enable the EPEL package repository on the hosts in the "web" group using the yum module.

   -  CentOS systems use the latest epel-release package
    - RHEL systems should use https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm
    - Create inventory groups app and web
- Status:

 8)set a cron on ansible control machine that will run every 1 minute , and perform below tasks
    

- execute ansible adhoc commands on client machines (cannot be control machine) , to create a file in /var/log/ninja_name on all the client nodes, append system_hostname [:space:] system_time in the file every 1 minute using ansible facts.

- Status:
