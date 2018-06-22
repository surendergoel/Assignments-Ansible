# The Assignment

- Create 5 users with password, and these five users should have same permissions for a directory named ninja.(Directory can be created with the 5 users permmission.)

- Create ssh key for each user so that all those 5 users will be able to login through ssh.
  - Status- [user_create_run](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/create%20user%20run.png) , [create_user.yml](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Playbooks/create_user.yml)

- Creat Logical Volume in any node machine.

- need to installl lvm2 first using ansible.

- Create ext4 type File System on the newly created logical volume.

- Mount newly created file system.
  - Status: [lvm.yml](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Playbooks/lvm.yml)
  - Issue: there is some issue in the playbook, will resolve it soon.
