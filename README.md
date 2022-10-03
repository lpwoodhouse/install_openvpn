# Ansible Play: install-openvpn

### <sub-heading>

This play is for installing the openvpn client and tailoring it for an ExpressVPN connection.

## Requirements

community.general<br>
ansible.posix

## Role Variables

Default variables for the install_openvpn role are listed below (see ```defaults/main.yml```)<br>
Values for the variables can be found by going to ExpressVPN manual setup instructions at https://www.expressvpn.com/setup#manual

```shell
auth:
  - <expressvpn_manual_setup_username>
  - <expressvpn_manual_setup_password>
location: <expressvpn_connection_location>
# location examples include: usa-sanfrancisco, usa-washingtondc, usa-denver, canada-montreal, uk-london, switzerland, hongkong-1, india-sg, malaysia
```
## Dependencies

None

## Example Playbook
```yaml
    - hosts: all
      roles:
        - install-openvpn
```

## License

MIT

## Author Information

This role was created in 2022 by [Lee Woodhouse](https://www.leewoodhouse.com/)
