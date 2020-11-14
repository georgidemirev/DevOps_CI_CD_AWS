# DevOps CI/CD pipeline with AWS EC2

------
Idea - Every time when we push new code in some repo, it should be deployed automaticallwithout any manual job.
------

Create Ubuntu EC2 instance for K8s management server and setup the K8s

Setup the K8s cluster on AWS with kops

Create the deploy and service yml files

......

Create EC2 for Ansible server and setup

Create the files for the playbooks

Create the Dockerfile

........

Create EC2 for Jenkins server and setup

Create job for CI and another one for CD 
-CI job is looking for new code push in some repository and building the image and pushing it to Docker hub (from Ansible playbook)
-CD job for kubernetes deployment running the deploy and service yml files (from Ansible playbook)
-add CD job in the CI job

Now every time when we push new code in the configured branch in the repo, 
the CI job will take that and run itself, afterwards running the CD job and 
Deploying the new app on the K8s cluster



