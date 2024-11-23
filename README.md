Install Wazuh Agent
===================

Set up the Wazuh agent using the [packages list](https://documentation.wazuh.com/current/installation-guide/packages-list.html) and register it to the Wazuh server.

Requirements
------------

- Ansible must be installed.
- Update variables to match your environment.
- Create an inventory file.

Role Variables
--------------

- `download_url`: The URL to download the package, as specified in the [Wazuh official documentation](https://documentation.wazuh.com/current/installation-guide/wazuh-agent/index.html).
- `local_path`: The local path where the package is downloaded before being installed on the VPS.
- `remote_copy_path`: The remote path where the package is copied and extracted for installation.
- `wazuh_manager`: The domain or IP address of the Wazuh server that the agent will connect to.

Example Playbook
----------------

```bash
ansible-playbook setup_wazuh.yml -i your_inventory.ini
```
License
-------

[Detail](./LICENSE)

Author Information
------------------

[Fat2Fast](https://github.com/fat2fast)