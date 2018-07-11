## The Assignment

1. List All the open ports on the node machines and store the output in seprate files named with the hostname of the machine on the ansible master.
```sh
$ ansible 192.168.33.30 -m setup | grep hostname | awk '{ print $2 }'
$ ansible 192.168.33.30 -m shell -a "netstat -l" >> /home/sudipt/ubuntu-xenial.txt
```
![hostname](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Day-9/Media/hostname.png)
![file](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Day-9/Media/file.png)
1. check if open ssh server is there or not on the machine.
```sh
$ sudo netstat -natp | grep sshd
```
![open-ssh](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Day-9/Media/open%20ssh.png)

2. disable all ports other than 22 on the node machines.
![disable-port](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Day-9/Media/disable.png)

[disable_port.yml](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Day-9/port.yml)


3. Enable only port 8080 and 8081 on the node machines.
![enable](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Day-9/Media/enable-port.png)

[enable_port.yml](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Day-9/enable_port.yml)

4. Again Check for open ports and append in same file with current date and time.
```sh
sudo ufw status
```

![status](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Day-9/Media/status.png)
