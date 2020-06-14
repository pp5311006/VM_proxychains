# VM_Proxychains

1. Download proxychains4
2. Enable v2ray from host PC(Your real OS)
3. Enable v2ray software to allow local network connections
4. From you host OS, check your IP address in order for VM to listen to
5. Edit /etc/proxychains.conf distable random_chain, select dynamic chain
6. Add: socks5 192.168.1.102 10808 to this file also, delete default conf
7. Make sure in /usr/bin/proxychains, the libproxychains.so.3 file is in the
   correct location
8. Make sure in /usr/lib/proxychains/proxyresolv, the DNS_SERVER is correct.
   ex: DNS_SERVER=87.118.85.241
9. Disable all the system proxy settiings by Win + proxy search
10.Type proxychains4 firefox google.com and check result
