# Kubernetes cluster creator with Ansible


## 1. Install Ansible

Instructions: https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#installing-ansible-on-ubuntu

TODO: just try `apt install ansible`


## 2. Configure

1. Copy the content of `poc-ansible-kubeadm/for-etc-ansible/ansible.cfg` to `/etc/ansible/ansible.cfg`.
    ```bash
    sudo bash -c  "echo '`cat for-etc-ansible/ansible.cfg`' >> /etc/ansible/ansible.cfg"
    ```

1. Prepare a hosts file based on the example of `hosts.example` file.




## X. Usage

```bash
ansible-playbook -v install.yml
```
