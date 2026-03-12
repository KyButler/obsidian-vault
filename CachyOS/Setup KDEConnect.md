
You have to manually allow these through the firewall to be able to connect devices.

```
sudo ufw allow 1714:1764/udp

sudo ufw allow 1714:1764/tcp

sudo ufw reload
```