# Ansible
Repository of all the required playbook.

This repository used to install/uninstall services on onpremise server.

# Sample

```bash
ansible-playbook -i sample-inventory.yml sample.yml --extra-vars "action=install"
ansible-playbook -i sample-inventory.yml sample.yml --extra-vars "action=uninstall"
```

## Install

```bash
ansible-playbook -i inventory.yml grafana.yml --extra-vars "action=install"
ansible-playbook -i inventory.yml loki.yml --extra-vars "action=install"
ansible-playbook -i inventory.yml victoriametrics.yml --extra-vars "action=install"
ansible-playbook -i inventory.yml otel.yml --extra-vars "action=uninstall"
```

## Uninstall
```bash
ansible-playbook -i inventory.yml grafana.yml --extra-vars "action=uninstall"
ansible-playbook -i inventory.yml loki.yml --extra-vars "action=uninstall"
ansible-playbook -i inventory.yml victoriametrics.yml --extra-vars "action=uninstall"
ansible-playbook -i inventory.yml otel.yml --extra-vars "action=uninstall"
```