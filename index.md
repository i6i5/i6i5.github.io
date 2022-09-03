# i6i5 site

## Hacking

### Monitor mode

#### Alfa AWUS036NHA 2.4 Ghz USB Wireless Adapter


#### Alfa AWUS036ACH 2.4 & 5 Ghz USB Wireless Adapter

Fix interference with monitormode
```bash
sudo airmon-ng check kill
```

Set interface down
```bash
sudo ip link set wlan0 down
```


Set monitor mode
```bash
sudo iw dev wlan0 set type monitor
```

Set interface up
```bash
sudo ip link set wlan0 up
```