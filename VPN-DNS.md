VPN (Virtual Personal Network)
DNS (Domain Name Server)

**wwww.vpnbook.com** kali içine VPN indirmemizi sağlar

**openvpn vpnadı** -> vpn dosyasını açar

**service network-manager restart** -> internet sunucularını resetler

#Kali DNS Ayarları Değiştirme

**nano /etc/dhcp/dhclient.conf** içindeki **prepentt name servers** değiştirmemiz gerekir

Google DNS-> 8.8.8.8 ya da 8.4.4.8
Cloudflare -> 1.1.1.1. ya da 1.0.0.1

#DNS sızıntı testi için

www..dnsleaktest.com
