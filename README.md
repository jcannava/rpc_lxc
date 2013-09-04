rpc_lxc
===

Uses a combination of ansible and Rackspace Public cloud to deploy a version of the Rackspace Private cloud
using lxc containers.

Prerequisites:
---
- requires pyrax library (pip install pyrax)
- requires ansible (pip install ansible)

Usage:
---
- Review group_vars/all and adjust for your setup
- Create a config file (~/.ansible_rax_creds) to hold RAX cloud credentials, see ansible_rax_creds.cfg
- Create a hosts file, see hosts
- run ansible-playbook -i hosts rax_lxc.yml
