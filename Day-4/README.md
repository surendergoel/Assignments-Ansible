# The Assignment

Create an Ansible playbook that targets members of the "app" group has the following state:

- The tomcat7 is installed in all host
- Has the war file in webapps folder specified in appwar.
- Tomcat is started on each host.
   - Status: [playbook1](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/playbook1.png) , [sample10](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/sample10.png)  , [sample20](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/sample20.png) , [Playbook.yml](https://github.com/sudiptninja/Assignments-Ansible/tree/master/Playbooks)
   - Learning: Learned about playbooks, its basic syntax, about YAML language. And sequential way to deploy war file using Ansible.


While developing the playbook use the --syntax-check to check your work and debug problems. Run your playbook in verbose mode using the -v switch to get more information on what Ansible is doing. Try -vv and -vvv for added verbosity. Also consider running --check to do a dry-run as you are developing.
