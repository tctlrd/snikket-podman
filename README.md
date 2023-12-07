## snikket-podman

Edit the configmap in the snikket-podman.yml and then deploy it like:

```
sudo podman play kube snikket-podman.yml
```


### Create an admin account

To create your first account, create an invitation with:

```
./scripts/new-invite.sh --admin --group default
```

Open the link in a browser. If you are on a desktop, you can use
tap the "Not on mobile?" button to display a QR code that can be
scanned with your mobile device.

During the account creation process you will choose a username and
password. Your Snikket address will be `<your username>@<your domain>`.
You can use this address and password to log into the web administration
page for the service.