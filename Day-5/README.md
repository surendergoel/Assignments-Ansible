# The Assignment

All needs to be done using ansible modules with jenkins There will be three jenkins jobs, Provisioning, Build, Deployment.

- Provisioning:-

   - Provision application servers, for example - java, tomcat are required for a java project.
     
   - This job will be a separate job and can be executed to any machine on requirement.
       - Status: [provision_configure](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/provision_configure.png) , [provision_output](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/provision_output.png) , [provisioning.yml](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Playbooks/Provisioning.yml)
       - Learning: Learned to use ansible plugin in jenkins and calling playbook in jenkins.
       

            Build and Deployment Job will be in downstream relationship.

- Build:-  Build any Project - can be java or any other language using jenkins.
  - Status: [build_configure](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/build_configure.png) , [build_output](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/build_output.png) , [build.yml](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Playbooks/build.yml)
  - Learning: Learned to install maven by downloading it rather than as a package installation, and using git module to clone the repo. building the code and clean compile the code by using playook.

- Deployment:-

    - Create a down stream deployment job to the build job .
    - In the deployment job , deploy the artifact (war in case of java) to the application server (tomcat/joboss) using ansible in the downstream job.
    - Ansible play book will include health check also, (status code == 200) , if health check fails, job should also fail.
      - Status: [deploy_configure](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/deploy_configure.png) , [deploy_console](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/deploy_console.png) , [deployment.yml](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Playbooks/deployment.yml)
      -  Learning: Learned about the limitations of copy module, and the concept of health checkup of a url and using uri module.
      - Issue: [downstream_config](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/deploy_error2.png) , [downstream console](https://github.com/sudiptninja/Assignments-Ansible/blob/master/Media/deploy_error1.png) . The deployment job is running successfully until it is triggered as downstream job of build job.
     
     
     
     - References - https://scriptcrunch.com/check-application-status-using-ansible/   for uri module
