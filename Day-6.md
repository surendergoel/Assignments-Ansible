# Assignment

    Create an Ansible playbook to rotate ssh keys. Explaination - Replacing the keys you’re currently using with
    new keys, and removing the ability for old keys to be used to log into your systems.

-   Create a new key
    - Status: [new_key](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/key%20new.png) 
-  Add new key to authorized_keys files on your nodes
   - Status: [adding_keys](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/key%20run%20playbook.png) , [older-keys](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/key%20previous.png) , [rotate_keys.yml](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Playbooks/rotate_keys.yml)
- Test new key 
  - Status: [new_keys](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/key%20new%20authorized.png)
- Remove previous keys from authorized_keys files on your nodes.
- again test the connectivity with the new keys.
  - Learning:  Learned to use authorized keys module, and replacing host's keys from nodes.

