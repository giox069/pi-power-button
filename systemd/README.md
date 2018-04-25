## systemd unit file for pi-power-button

Use this systemd unit file to start `listen-for-shutdown.py` at boot in systemd system (recent Raspbian).

To install:
1. Download the [listen-for-shutdown.service](https://raw.githubusercontent.com/giox069/pi-power-button/master/systemd/listen-for-shutdown.service) file
2. Copy the downloaded file to /etc/etc/systemd/system/:
```sudo cp listen-for-shutdown.service /etc/etc/systemd/system```
3. Add it to systemd, set it to autostart and start it
```
sudo systemctl daemon-reload
sudo systemctl enable listen-for-shutdow
sudo systemctl start listen-for-shutdown
```

