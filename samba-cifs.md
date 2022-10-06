# SAMBA/CIFS mounts

## CLI mounting

Mount a samba cifs share from the CLI with
```bash
sudo mount -t cifs -o user=<username>  //<ip address>/serverpath /local/path 
```

you will be prompted for your password on the server

To map your username and group to the server use
```bash
sudo mount -t cifs -o user=<username>,uid=`id -u`,gid=`id -g` //<server url>/serverpath /local/path
```
