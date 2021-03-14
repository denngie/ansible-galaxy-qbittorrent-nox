qbittorrent_nox
=========

Installs qBittorrent headless version on your Ubuntu server

Requirements
------------

TBD

Role Variables
--------------

Default variables:
```yaml
content_path: Base path for your torrents, media files and scripts
qbt_version: PPA to use, stable or unstable
qbt_user: local user running qbittorrent-nox 
qbt_seed_days: How many days of seeding before torrent is removed
qbt_port: port used by qBittorrent
```

Dependencies
------------

Not a dependency but this role is intended to be used with my other role denngie.flexget_daemon

Example Playbook
----------------

```yaml
---
- name: Apply qbittorrent-nox role
  hosts: qbittorrent-server
  roles:
    - denngie.qbittorrent_nox
```

License
-------

MIT
