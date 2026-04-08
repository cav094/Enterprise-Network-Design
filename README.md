# Enterprise-Network-Design

# Enterprise Network Lab (VLAN + VRRP)

##  Overview

Designed and implemented a **redundant enterprise network** in GNS3 using MikroTik devices.

The lab demonstrates VLAN segmentation, inter-VLAN routing, and high availability using VRRP.

---

##  Architecture

* Dual Core Layer 3 switches (redundancy)
* Distribution and Access layers
* End devices in multiple VLANs
* Internet connectivity via router/firewall

---

##  VLAN Design

| VLAN | Purpose    | Subnet          |
| ---- | ---------- | --------------- |
| 100  | IT         | 192.168.10.0/24 |
| 200  | Finance    | 192.168.20.0/24 |
| 99   | Management | 192.168.99.0/24 |

---

##  High Availability (VRRP)

* Virtual gateways:

  * 192.168.10.1
  * 192.168.20.1
* Automatic failover between core switches
* No downtime during core failure

---

##  Key Configurations

* VLAN trunking across all switches
* Inter-VLAN routing on L3 Core switches
* VRRP for gateway redundancy
* End-to-end connectivity validation

---

##  Testing

* Inter-VLAN communication successful
* PCs use virtual gateway (.1)
* Failover test: network remains operational when primary core is down

---

##  Topology

<img width="1237" height="788" alt="vlan1" src="https://github.com/user-attachments/assets/805107a2-83b4-41bf-afd4-9b4e6e2ae198" />


---

##  Skills Demonstrated

* Enterprise network design (3-tier architecture)
* VLAN & trunk configuration
* High availability (VRRP)
* Network troubleshooting and fault isolation

---

## 👤 Author

Kelvin Zakayo
Network Administrator (MikroTik | Cisco | Routing | VLAN | MPLS)
