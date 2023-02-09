This playbook uses four tasks to accomplish the task. The first task updates the package cache, the second task installs the sysstat package, the third task copies the custom sysstat configuration file to the machine, and the fourth task restarts the sysstat service to apply the changes.

Make sure that the custom sysstat configuration file, sysstat.conf, is located in the same directory as the playbook file.

This playbook assumes that the machines are running a Debian-based operating system and that the apt and service modules are available. If your machines are running a different operating system, you may need to modify the playbook accordingly.

You can run this playbook using the following command:
ansible-playbook -i <inventory_file> <playbook_file>.yml

Replace <inventory_file> with the path to your inventory file and <playbook_file> with the name of the playbook file.