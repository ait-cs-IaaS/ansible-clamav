# ClamAV-Ansible-Role

This ansible installs the clamav-command-line scanner and
schedules a cronjob for it.

# Defaults

```
clamav_packages:
        - clamav

clamav_minute: "30"
clamav_hour: "08,20"
```

# Usage

```
- hosts: localhost
  roles:
        - clamav
  vars:
# run daily at 09:45
        clamav_minute: "45"
        clamav_hour: "09"
```
