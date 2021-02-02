This ansible playbook will install R1soft agent and server on centos 7. Please follow the steps

Step 1 
Create r1soft server and r1soft agent on centos 7

Step 2
Give access (public/private key matching) from ansible to the R1soft server and agent
 
Step 3 
Create r1soft.repo file for r1soft server and agent

Step 4 
Add hosts to the inventory file: vi /etc/ansible/hosts

cat /etc/ansible/hosts
[r1soft-server]
IP of r1soft server

[r1soft-agent]
IP of r1soft-agent

Step 5 
clone the ansible-playbook from GitHub and get into r1soft-ansible file

git clone https://github.com/stoktobekova/r1soft.git
cd r1soft-ansible

Step 6
Ansible-playbook r1sof-server.yml
and ansible-playbook  r1sof-agent.yml

Step 7
Copy IP address of server and put on browser with :8080 port 

Step 8
Add agent machine and check connection

Step 8
Add volumes for backups and run backup depending how often backups should be running.
