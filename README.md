# Ansible Role: clamav

This Ansible Role installs the clamav-command-line scanner and schedules a cronjob for it.

## Defaults

```yaml
clamav_packages:
  - clamav
```

```yaml
clamav_minute: "30"
```

```yaml
clamav_hour: "08,20"
```

## Usage

```yaml
- hosts: localhost
  roles:
    - clamav
  vars:
    # run daily at 09:45
    clamav_minute: "45"
    clamav_hour: "09"
```
