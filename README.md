# Ansible-pull
a project for storing Ansible playbooks to be pulled and executed locally by slave servers

in push mode, we install ansible on the master server only which pushes playbooks to hosts and execute them with some user we configure

in pull mode, we install ansible on hosts wich then pulls the git repo periodically to check for playbooks to be executed and pull and execute them locally on itself (by default ansible-pull wil look for a playbook named local.yaml in the repo and execute whatever tasks in it locally)
