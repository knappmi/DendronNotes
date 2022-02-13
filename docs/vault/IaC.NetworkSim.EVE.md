---
id: I5N4Y3V4xp1uMreTPYrVu
title: EVE
desc: ''
updated: 1644722890604
created: 1644713350394
---

## **Advanced config to brige connection:**

### To config nat:
_iptables -t nat -A POSTROUTING -s (subnet)(/netmask) -o pnet0 -j MASQUERADE_

### Verify with:
_iptables -L -nv -t nat_


## **To enable ipforwarding:**
### Change sysctl.conf
_nano etc/sysctl.conf_

### Uncomment the following:
_net.ipv4.tcp\_syncookies = 1_

## When depolying images, change the adapter from vmx


