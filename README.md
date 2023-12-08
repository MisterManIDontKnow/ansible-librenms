# ansible-librenms
Deploy LibreNMS on a CentOS server.

Requires:
- files
  1. vars/vault.yml #See [ansible best practices](https://docs.ansible.com/archive/ansible/2.3/playbooks_best_practices.html#variables-and-vaults)
  2. templates/\<whatever your environment dictates are the appropriate end configurations\>

- Updating the vars/main.yml with the appropriate values for variables:
  1. ansible_hostname
  2. latest_release
  3. LIBRENMS_GROUP_ID
