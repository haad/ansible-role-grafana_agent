# Ansible Role: Grafana Cloud Agent

![Ansible Lint](https://github.com/haad/ansible-role-grafana_agent/workflows/Ansible%20Lint/badge.svg?branch=main) ![Ansible Role](https://img.shields.io/ansible/role/52768?style=plastic) ![Quality Score](https://img.shields.io/ansible/quality/52768) ![Downloads](https://img.shields.io/ansible/role/d/52768?style=plastic)

Installs [Grafana Cloud Agent](https://github.com/grafana/agent) on RedHat/CentOS or Debian/Ubuntu servers to collect observability data and sends it to [Grafana Cloud](https://grafana.com/products/cloud/).

This role installs and configures the latest version of [Grafana Cloud Agent](https://github.com/grafana/agent) from [GitHub releases](https://github.com/grafana/agent/releases). It also creates a [systemd service to manage the agent](https://grafana.com/docs/grafana-cloud/agent/agent_as_service/).

It optionally installs [Promtail](https://grafana.com/docs/loki/latest/clients/promtail/), which is an agent which ships the contents of local logs to [Grafana Cloud](https://grafana.com/products/cloud/) ([Loki](https://grafana.com/oss/loki/)).

**WHY**? => [Monitoring your home lab devices in the cloud for free](https://nleiva.medium.com/monitoring-your-home-lab-devices-in-the-cloud-for-free-54c4d11ac471)

## Requirements

None. Other than an account on [Grafana Cloud](https://grafana.com/products/cloud/) -> [Create account](https://grafana.com/signup/cloud/connect-account).

## Role Variables


## Dependencies

None.

## Example Playbook

    - hosts: server
      roles:
        - { role: haad.grafana_agent }

## License

GPL-3.0 License

## Author Information

This role was created in 2021 by [Nicolas Leiva](https://github.com/nleiva).
This role was refactored/updated in 2022 by [Adam Hamsik](https://github.com/haad).
