1. The 'system' folder contains information about the usage of Ansible on Linux nodes
2. The user 'automation' is created on all nodes (control node and managed nodes). This user will run ansible ad-hoc commands and playbooks on control node.
3. Under user 'automation' home directory ($PWD - /home/automation), create a new folder for the ansible project called 'ansible_labs'. This folder 'ansible_labs' is the place to store other ansible files/configs (ansible.cfg, inventory 'hosts' file...)
4. the following outputs are what have been written previously at bullet point #3:\
  **[automation@netsyslab~]$** pwd\
  /home/automation\
  **[automation@netsyslab~]$** ls\
  ansible-labs\
  **[automation@netsyslab~]$** cd ansible-labs/\
  **[automation@netsyslab ansible_labs]$** ls\
  ansible.cfg hosts\
  **[automation@netsyslab ansible_labs]$** ansible --version\
  ansible [core 2.14.17]\
    config file = /home/automation/ansible-labs/ansible.cfg\
    configured module search path = ['/home/automation/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']\
    ansible python module location = /usr/lib/python3.9/site-packages/ansible\
    ansible collection location = /home/automation/.ansible/collections:/usr/share/ansible/collections\
    executable location = /usr/bin/ansible\
    python version = 3.9.21 (main, Dec 05 2024, 00:00:00) [GCC 11.5.0 20240709 (RED HAT 11.5.0-2)] (/usr/lib/python3)\
    jinja version = 3.1.2\
    libyaml = True\
