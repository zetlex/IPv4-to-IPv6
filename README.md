# IPv4-to-IPv6
Convert your internet traffic from IPv4 ➜ IPv6.
Auto-installer will be made in the future.

## Requirements
- Ubuntu Server 20.04
- Dedicated IPv4 and IPv6 Subnet
<br>
Can be purchased from https://bytehosting.cloud for 2.99€ / month.<br>
1vCPU • Xeon E5 <br>
4GB • RAM <br>
30GB • NVMe Storage <br>
1 • IPv4 Address <br>
1 • IPv6 /64 Subnet <br>
1TB • Bandwidth<br>

## Installation
`sudo apt update && sudo apt upgrade -y sudo apt-get install git`<br>
`sudo git clone <https://github.com/Nyr/openvpn-install.git>`<br>
`sudo cd openvpn-install/`<br>
`sudo chmod +x [openvpn-install.sh](<http://openvpn-install.sh/>)`<br>
`sudo ./openvpn-install.sh`<br>

## Configuration (Important)
`sudo nano /etc/openvpn/server/server.conf`<br>
Change `proto udp` to `proto udp6`.
`sudo systemctl restart openvpn`

## Connecting
Copy the .ovpn file to your device and connect to it using OpenVPN Connect.<br>
https://openvpn.net/client/client-connect-vpn-for-windows/
