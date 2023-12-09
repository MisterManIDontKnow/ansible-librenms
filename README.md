# ansible-librenms
Deploy LibreNMS on a CentOS server.

Requires:
- Specifying a tag:
  1. **update** can be for upgrades or general migrations.
  2. **install** for a fresh deployment
  
- Files:
  1. **vars/vault.yml** See [ansible best practices](https://docs.ansible.com/archive/ansible/2.3/playbooks_best_practices.html#variables-and-vaults)
  2. **templates/\<whatever your environment dictates are the appropriate end configurations\>**
  3. **files/id_rsa** This is the private key of the old librenms server librenms user if migrating (update tag)
  4. **files/releases/latest/** This is only used if using the install tag

- Updating the vars/main.yml with the appropriate values for variables:
  1. **ansible_hostname**
  2. **latest_release** This is used only if using the install tag
  3. **LIBRENMS_GROUP_ID**
  4. **distribution_min_version**
  5. **distribution_name**
