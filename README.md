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

1. Make sure `known_hosts` of the host machine contains the fingerprints of all VMs

1. Run the playbook
    ```bash
    ansible-playbook -v install.yml
    ```
1. BONUS: An example nginx deployment

    source https://kubernetes.io/docs/tasks/run-application/run-stateless-application-deployment/
    ```bash
    kubectl apply -f https://k8s.io/examples/application/deployment.yaml
    ```