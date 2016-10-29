# Setup CoreOS Cluster #

## Intro ##

This playbook is an example and creats a CoreOS cluster with 3 nodes with a
mongodb service and using an NFS share for persistent data.  

## Using ##

- Crate a VM with NFS export.
- Create KVM virtual machines and note the IP addresses.
- Rename the "hosts.example" in "hosts" and modify the entries (with the IP addresses).
- Enter:

```
ansible-playbook -i ./hosts ./cluster-setup.yml
```
