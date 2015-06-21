# louisvill.io-ansible
[Ansible](http://docs.ansible.com/index.html) playbooks for setting up [Louisville.io](http://louisville.io) servers.

Initial server setup:
```
ansible-playbook -i ansible_hosts production.yml
```

Deploy site:
```
ansible-playbook -i ansible_hosts deploy.yml
```
