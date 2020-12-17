# unchain

Install script for SoftEther VPN on GL-AR300M

## Requirements

- 1x Debian 9 or 10, Cloud server or Docker image

- 1x GL-AR300M Mini Router

## Install

1. Install Server (Debian 9 or 10):

```
chmod +x install-server.sh
./install-server.sh
# Set a password
```

2. Install Client (GL-AR300M):

```
# Make sure internet is connected
opkg install git-http
chmod +x install-client.sh
./install-client.sh
# Enter server IP and password
```

## Use

- portable, built for traveling, public Wi-Fi, and remote work
- easy to use:
  ^ Turn VPN on/off with the switch button
  ^ Connect any type of device to the box and enjoy your unrestricted network via LAN or WLAN
  ^ Connect wirelessly to public hotspots (see 'Repeater mode')
`
You can permanently disable the process with

```
/etc/init.d/sevpn disable
```

or re-enable with

```
/etc/init.d/sevpn enable
```

## Troubleshooting

- Turn off 'DNS Rebinding Attack Protection' if you encounter problems with obtaining the captive portal from public hotspots

## Info

Protocol: TLS (SoftEther VPN)

Server port: TCP 443
