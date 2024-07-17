# Ansible Role: Kali Apps ([Ludus](https://ludus.cloud))

An Ansible Role that will install Pentesting applications onto a Kali Linux minimal OS

## Requirements

None.

## Role Variables

None.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: hosts
  roles:
    - PrymalInstynct.ludus_kali_apps
```

## Example Ludus Range Config

```yaml
ludus:
  - vm_name: "{{ range_id }}-kali-01"
    hostname: "{{ range_id }}-kali-01"
    template: debian-12-x64-server-template
    vlan: 10
    ip_last_octet: 1
    ram_gb: 4
    cpus: 2
    linux: true
    roles:
      - PrymalInstynct.ludus_kali_apps
```

## License

GPLv3

## Author Information

This role was created by [PrymalInstynct](https://github.com/PrymalInstynct), for [Ludus](https://ludus.cloud/).
