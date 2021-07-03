# swarm_infrastructure
Swarm Infrastructure deployed on proxmox with ansible and glusterFS

Working:

createlxc.yml deploys 3 ubuntu LXC with minimal configuration to a proxmox hypervisor. 

installDocker.yml install on the deployed LXCs Docker

ToDo:

Use Vault for pub RSA key and api passwords

createSwarm.yml create a swarm cluster from the nodes

createglusterFS.yml create a glusterFS across the nodes

glusterFS has to be configured as primary FS for Docker

Required Ansible libraries:
community.docker
community.general.proxmox
gluster.gluster
