# 🛠️ Ansible Automation

This repository contains real-world Ansible playbooks used to automate server configuration and application deployment.

## 📁 Structure

- `playbooks/`: Main Ansible playbooks
- `roles/`: Reusable roles (to be added)
- `inventories/`: Inventory files for different environments
- `group_vars/`: Group variable files

## 🚀 Sample Playbook

```yaml
- name: Install and start Nginx
  hosts: web
  become: yes
  tasks:
    - name: Install Nginx
      apt:
        name: nginx
        state: present