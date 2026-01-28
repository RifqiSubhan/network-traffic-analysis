## Network Discovery and Service Enumeration (Nmap)

This simulation demonstrates a local network reconnaissance process performed in a controlled lab environment to identify active hosts and exposed services.

### Lab Environment
- Scanner (Attacker): 10.93.109.99
- Target Host: 10.93.109.76
- Network Scope: 10.93.109.0/24

---

### Phase 1: Host Discovery
An initial ping scan was conducted to identify active hosts within the local subnet.

```bash
nmap -sn 10.93.109.0/24

Phase 2: Service and System Enumeration

After identifying an active host, a more detailed scan was performed against the target to enumerate services and system information.
nmap -A 10.93.109.76 -v
Techniques applied:

Service version detection

OS detection

Default NSE scripts

Phase 3: Vulnerability Assessment (Simulation)

Nmap NSE vulnerability scripts were executed to identify potential security issues and misconfigurations.

nmap --script vuln 10.93.109.76 -v

Disclaimer:
All scans were conducted on systems owned and controlled by the author for educational and analysis purposes.


### Evidence
![Nmap Service Enumeration](screenshots/nmap_service_enum_10.93.109.76.png)
