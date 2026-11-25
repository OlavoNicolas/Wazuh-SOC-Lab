
# Wazuh All-in-One — Installation

## 1. Environment

- OS: Ubuntu Server 26.04 LTS
- Deployment: All-in-One
- Wazuh version: 4.14
- CPU: 2 vCPU
- RAM: 8 GB
- Storage: 100 GB NVMe

## 2. Architecture

The following components were deployed on the same VPS:

- Wazuh Server / Manager
- Wazuh Indexer
- Wazuh Dashboard
- Filebeat

## 3. Installation

The official Wazuh installation assistant was used.

```bash
curl -sO https://packages.wazuh.com/4.14/wazuh-install.sh
sudo bash ./wazuh-install.sh -a
```

## 4. Validation

- [x] Wazuh Manager service active
- [x] Wazuh Indexer service active
- [x] Wazuh Dashboard service active
- [x] Filebeat service active
- [x] Dashboard accessible through Windows browser
- [x] Initial resource consumption checked

## 5. Security considerations

- Dashboard access restricted by firewall rules.
- Indexer API not exposed publicly.
- Wazuh API not exposed publicly.
- Credentials stored securely.

## 6. Compatibility note

The deployment was performed on Ubuntu Server 26.04 LTS.
This OS version was not listed among the officially supported
operating systems for Wazuh 4.14 in the documentation consulted.

The installation completed and initial service validation
was successful. Compatibility and long-term stability
remain subject to further testing.

## 7. Current status

Wazuh All-in-One deployed and accessible.
Windows endpoint integration is pending.
