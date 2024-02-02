Role Name
=========

The rhone playbook & roles install and configure Red Hat Identity Management. This includes promoting a a Windows 2022 to a DC and creates both users and groups for use in demonstrating the use of Ansible to install and configure RH IdM with an AD trust, IDP, and DNS.


Requirements
------------

This collection uses the redhat.rhel_idm and redhat.rhel_system_roles collections from console.redhat.com
To install these collections you will need to log in to console.redhat.com and run:
  ansible-galaxy collection install redhat.rhel_idm and ansible-galaxy collection install redhat.rhel_system_roles
To run the Windows roles, you will need to install the python3-winrm package and the following Ansible modules:
  ansible-galaxy collection install ansible.windows
  ansible-galaxy collection install community.windows
If you are running older versions of Windows, 2016 and earlier, zou must also run the WinRM Memory Hotfix and WinRM Setup scripts on the Window server to allow WinRM to accept connections from Ansible.
The doc is here: https://docs.ansible.com/ansible/latest/os_guide/windows_setup.html


Role Variables
--------------

Variables are in two places: inventory and secret.yml
  inventory holds all public variables.
  secret.yml holds all the sensitive variables.


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.


Author Information
------------------

Mike Ralph, Sr Technical Account Manager: https://rover.redhat.com/people/profile/mralph
