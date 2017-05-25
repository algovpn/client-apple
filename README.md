algovpn.client-apple
====================

Apple client mobileconfig generation.

Requirements
------------

The role requires that the algovpn.vpn role or KeyManager ansible
module be run before this role. See tests/test.yml for an example of
using this role externally.

Role Variables
--------------


| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `apple_on_demand_wifi` | false | Toggle on demand WiFi support.|
| `apple_on_demand_cell` | false | Toggle on demand cellular support.
| `wifi_exclusion_networks` | [] | A list of WiFi networks to exclude for on demand |
| `client_config_output_folder` | cwd | Output folder of the generated config files |

Dependencies
------------

algovpn.vpn

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: algovpn.client-apple, apple_on_demand_wifi: True }

License
-------

MIT

Author Information
------------------

AlgoVPN