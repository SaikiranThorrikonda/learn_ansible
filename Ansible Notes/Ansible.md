What is Ansible?
 -  Real life use cases
  - Ansible Components (-Modules & Playbooks)
   - Ansible with Docker

Why Ansible?
 - Its a tool to automate different IT Tasks.
 - Repetitive IT administration Tasks (like OS Upgrade in 100's of servers, firmware updates or other updates, patching, weekly system reboots, Backups, creating users & assigning permissions... etc.)
 - Imagine you have 10 servers running distributed app (microservices) or you want to update docker version on all those servers need manual commands by SSH on each server one by one {systemctl stop docker, upgrade docker, systemctl start docker}
 -  Ansible supports all OS platforms and cloud providers.
 - Ansible is Agentless. (Ansible is installed in the control machine then it connects all the target servers using SSH) this provides:- 
                                                                      - no deployment effort in the beginning setup
                                                                      -  no upgrade effort on the servers.
    ![[ansible_img.png]]
Ansible Use cases: 
  - Provisioning Environments
  - Configuration Management (OS, Security patches, installing databases)
  - Deploying containers, applications/ software etc.
  - Performing Compliance Checks
  - Installing Jenkins, deploying k8's clusters on any Cloud platform using Ansible

 How ansible works: Ansible Architecture

 Ansible works with modules (these modules are granular i.e, one module does one specific task only), Modules are the small programs that do the actual work, once they finish their task they get removed.
 
 Ex. One module to copy a file;
       One module to install Nginx Server;
       One module to start Nginx Server

 Modules are pushed from control machine to target machines
 those modules do their job on the target server and then get removed
 ![[module_img.png]]

Ansible has 100's of modules for different tasks which can be found here
https://docs.ansible.com/ansible/2.9/modules/modules_by_category.html

Ansible Integration with DevOps Tools:
https://www.ansible.com/integrations/devops-tools

Ansible uses YAML. (Hence it became so popular) which is super intuitive

while deploying a complex application, we need multiple modules to be performed
in a specific sequence














