1. The 'system' folder contains information about the usage of Ansible on Linux nodes
2. The user 'automation' is created on all nodes (control node and managed nodes). This user will run ansible ad-hoc commands and playbooks on control node.
3. Under user 'automation' home directory ($PWD - /home/automation), create a new folder for the ansible project called 'ansible_labs'. This folder 'ansible_labs' is the place to store other ansible files/configs (ansible.cfg, inventory 'hosts' file...)
