# 🧠 Automated BGP/OSPF Lab with Batfish & Ansible

This project simulates a multi-AS BGP/OSPF topology using Cisco IOL routers in PNETLab. It automates device configuration with Ansible and validates routing using Batfish and pybatfish.

## 🛠️ Tools Used

- PNETLab + Cisco IOL
- Ansible (for config push via templates)
- Jinja2 (config rendering)
- NAPALM / Netmiko (optional Python config delivery)
- Batfish (for BGP/OSPF validation)
- GitHub Actions (CI pipeline for validation)

## ✅ Features

- Automated rendering of startup configs using Ansible + Jinja2
- Push config to devices (or export for PNETLab import)
- Load configs into Batfish container
- Run automated checks (e.g., BGP session health, route leakage)
- CI/CD pipeline: auto-run Batfish tests on every code change
