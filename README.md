# ansible-vcenter

Playbook for deploying a ova template over VMware vCenter (vSphere), installing Nginx, MySQL and Wordpress.
Default Image: bionic-server-cloudimg-amd64
The Image will be downloaded by ansible playbook. The VM Harddisk will also be resized.

## Required Variables

Path: roles/vcenter/defaults/main.yml

* vcenter_hostname:
* vcenter_datacenter:
* vcenter_cluster:
* vcenter_datastore:
* vcenter_folder:
* vcenter_network:

Path: roles/vcenter/vars/main.yml

* vcenter_username:
* vcenter_password:

for security reasons this file can be encrypted using ansible-vault. then a vault-pass.txt file must be provided oder the password must be specified in the ansible command! 
