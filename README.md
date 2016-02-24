# til

- `upstart` files go into `/etc/init/file.conf`. Then `sudo start/stop/restart file`
- `systemctl` files go into `/etc/systemd/system/somefile.service`. Then `sudo systemctl daemon-reload` followed by `sudo systemctl start/stop/restart somefile`
- `systemctl --failed` to see units that failed
