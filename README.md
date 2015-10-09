# Multi Region VPN Connection Using OpenVPN
Connecting multiple regions together via a vpn connection using OpenVPN.

```
sudo su
apt-get update
apt-get install openswan strongswan git -y
cd /root
git clone https://github.com/andrewpuch/multi_region_vpn_connection.git
cp multi_region_vpn_connection/ipsec.sh /sbin
cp multi_region_vpn_connection/ipsec.secrets /etc
cp multi_region_vpn_connection/ipsec.conf /etc
chmod 744 /sbin/ipsec.sh
chmod 744 /etc/ipsec.secrets
chmod 744 /etc/ipsec.conf
```

Edit the files according to the tutorial.

```
service ipsec restart
```
