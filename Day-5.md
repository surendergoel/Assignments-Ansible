# The Assignment

All needs to be done using ansible modules with jenkins There will be three jenkins jobs, Provisioning, Build, Deployment.

- Provisioning:-

   - Provision application servers, for example - java, tomcat are required for a java project.
   - This job will be a separate job and can be executed to any machine on requirement.

            Build and Deployment Job will be in downstream relationship.

- Build:-  Build any Project - can be java or any other language using jenkins.

- Deployment:-

    - Create a down stream deployment job to the build job .
    - In the deployment job , deploy the artifact (war in case of java) to the application server (tomcat/joboss) using ansible in the downstream job.
    - Ansible play book will include health check also, (status code == 200) , if health check fails, job should also fail.
