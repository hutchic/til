# til

- `upstart` files go into `/etc/init/file.conf`. Then `sudo start/stop/restart file`
- `systemctl` files go into `/etc/systemd/system/somefile.service`. Then `sudo systemctl daemon-reload` followed by `sudo systemctl start/stop/restart somefile`
- `systemctl --failed` to see units that failed
- http://www.lexicallyscoped.com/2013/04/02/simple-init.d-script-for-ansible.html
- journalctl -u unit.servce
- remove accidentally commited sensitive data
```
git filter-branch --force --index-filter \
'git rm --cached --ignore-unmatch MISTAKES_WERE_MADE’ \
--prune-empty --tag-name-filter cat -- --all
```
