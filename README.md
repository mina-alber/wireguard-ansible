# WireGuard Ansible
![AUR](https://img.shields.io/aur/license/yaourt.svg)

![WireGuard Logo](./wireguard_logo.svg)

This Ansible playbook installs and configures the WireGuard server on `CentOS 7`. Everything is configurable all you need to do is to modify the `vars` file & the `hosts` file and you're ready to go.

## Requirements
This playbook tested on Ansible 2.5
## Installation
```sh
ansible-playbook -i hosts.ini wireguard.yml
```
## Role Variables
To configure the script before using it please check `./vars.yml`
```yml
wireguard_repo: "https://copr.fedorainfracloud.org/coprs/jdoss/wireguard/repo/epel-7/jdoss-wireguard-epel-7.repo"
wireguard_interface_ip: "10.0.0.1/24" # IPADDR/PREFIX
wireguard_port: "51820"
```

## TODOs
* [ ] Support Ubuntu
* [ ] Add and revoking users keys
* [ ] Test the playbook on Ansible old versions

## License
GPL v3.0

## How to Contribute
Fork > Do your magic > Test > Pull request
