RiotKit Universal Node
======================

Turns a typical cheap virtual node into a dockerized applications environment. Natively integrates with RiotKit's Harbor 2+ for webservices deployment.

First time setup
----------------

```bash
cp .env-dist .env
nano .env

rkd :setup
rkd :copy-host-defaults
```

Features
--------

- Structure and automation
- User accounts management
- Basic security (firewall ports, fail2ban, partial disk encryption)
- Extensibility
- Native integration with RiotKit Harbor
- Logs rotation and logs privacy management
- Inventory in separate GIT repository

Cheap node specification
------------------------

This set of playbooks needs to run at least on this specification:

- CPU: 1-4 cores
- RAM: 1-4 GB
- HDD: 20-40 GB SSD (including OS)
- OS: Ubuntu 16.04+ or latest Debian Stable or Latest Armbian
- Host type: Physical ARM or KVM
