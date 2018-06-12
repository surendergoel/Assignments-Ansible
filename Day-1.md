# Assignment
  - Use pip to install the ansible package and its dependencies to your control machine.
     - Status- https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/python%20pip.png
     - Learning : Pip is a package management system used to install python based repositories, like Ansible
- Display the Ansible version and man page to STDOUT.
     - Status-https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/ansible%20version.png
     - Learning : About different commands which could be used frequently
- Check all the possible parameters you need to know in ansible.cfg file.
    - Status- Done
    - Learning : About hosts, forks, inventory ,library, modules,etc. The parameters which a user can configure for the working of ansible.
- Ansible Inventory: Check the default inventory file for ansible control master and use inventory, run ansible ping commands on various inventory groups. Try this on minimum of two virtual machines.(You can use any of these Docker/Vagrant)
    - Status- https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/pingpong.png
    - Learning : In this we configure the ip addresses of the servers, which could be organized as groups.
- In ~/.ansible.cfg file (create the file if it doesn't exist already) do the following:
    - Status-Done
- Create a new directory ~/.ansible/retry-files and set retry_files_save_path to it.
    - Status-https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/retryfiles.png
    - Learning : In, general any software gives priority to access the config files as: 
        1.  ./ansible.cfg
        2.  ~/.ansible.cfg
        3.  /etc/ansible/ansible.cfg
It means the software will be configured in accordance with the priority set above.
- Set the Ansible system forks to 10
    - Status-https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/fork.png
    - Learning : Forks is the maximum no. of servers can be served in a single go.
    
    # Problem statement: Using Adhoc command

- Host a static website on minimum three hosts using inventory, content of static website is "Index page of Ansible assignment"
Document root /opt/html

    - Status- https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/webpage.png
    - Learning : How to configure servers for deploying a simple HTML file, using Ad-Hoc commands and copy modules. And configuring the path of HTML file in nginx in its configuration file.

- First do this manually and then with jenkins using ansible plugin or execute shell. only use ansible modules.
    - Status- Vagrant corrupted, jenkins lost

