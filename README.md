# Ansible Role: prometheus-pushgateway

An Ansible role that installs Prometheus Pushgateway on Ubuntu-based machines with systemd.

## Requirements

All needed packages will be installed with this role.

## Role Variables

Available variables are listed below, along with default values:
```yaml
prometheus_pushgateway_version: 0.3.1

prometheus-pushgateway_config_flags:
  'web.listen-address': '0.0.0.0:9091'
  'log.level': 'info'
```
## Dependencies

- UnderGreen.prometheus-exporters-common

## Example Playbook
```yaml
- hosts: node-pushgateway
  roles:
    - stephanfuchs.prometheus-pushgateway
```
## References
- https://github.com/UnderGreen/ansible-prometheus-node-exporter

## License

GPLv2
