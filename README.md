## snikket-podman

Edit the configmap in the snikket-podman.yml and then deploy it like:

```
$ sudo podman play kube snikket-podman.yml
```
### systemd service
To enable auto pod start on system restart and auto-update of containers run the snikket pod as a systemd service.  
The instructions are found here:  
https://docs.podman.io/en/latest/markdown/podman-generate-systemd.1.html#kubernetes-integration

Here is an example:
```
$ escaped=$(systemd-escape ~/snikket-podman.yml)
$ systemctl --user start podman-kube@$escaped.service
$ systemctl --user is-active podman-kube@$escaped.service
active
```
