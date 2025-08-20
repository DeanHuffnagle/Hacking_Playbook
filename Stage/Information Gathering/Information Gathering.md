## Nmap initial Scan - TCP
```bash
nmap $TARGET_IP -p- -T4 -oN initial_TCP_scan 
```
- Performs a TCP scan on all ports to get an initial list of all open ports.

---

## Nmap initial Scan - UDP
```bash
nmap $TARGET_IP -sU -T4 --min-rate 300 -oN initial_UDP_scan 
```
- Performs a UDP scan on top 100 ports to get an initial list of open UDP ports.
- **Note:** UDP scans take a long time.

---

## Nmap Aggressive Scan - TCP
```bash
nmap $TARGET_IP -p $TARGET_PORTS -A  -oN aggressive_TCP_scan 
```
- Performs an aggressive scan on all targeted ports.
- **Note:** when choosing ports, add at least one known closed port to aid with the OS detection.
- **Note:** Aggressive scans take longer, which is why we limit it to a more narrow list of ports (gathered from the initial scan).

---
