## snikket-podman

Edit the configmap in the snikket-podman.yml and then deploy it like:

```
$ sudo podman play kube snikket-podman.yml
```
### systemd service
To enable auto pod start on system restart and auto-update of containers run the snikket pod as a systemd service.  
The instructions are found here:  
https://docs.podman.io/en/latest/markdown/podman-systemd.unit.5.html#kube-units-kube
