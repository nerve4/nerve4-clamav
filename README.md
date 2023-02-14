# clamAV

An Ansible role that installs clamAV to CENTOS 7/8, Rocky9 and Ubuntu. More info about clamAV: [link](https://www.clamav.net/)


## Requirements

Make sure, you made your vars file with valid path to custom template or you can use Default vars.

You need `ansible 2.13.7` to run this module

The Role also use `community.general collection` module. To install it, use: `ansible-galaxy collection install community.general`. 


## Tasks descriptions

- main.yml - Run the OS check and run the relevant playbook
- rhel-install-clamav.yml - Deploy clamAV on Rhel
- ubuntu-install-clamav.yml - Deploy clamAV on Ubuntu
- configure-clamav.yml - Configure ClamAV


## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
- hosts: servergroup
  become: true
  become_user: lee

  vars_files:
    - vars/main.yml
    
  roles:
    - nerve4-clamav
```


## Maintainer Information
Lee | 2023