# Site-to-Site IPsec VPN and eBGP Dual-ISP

## **Overview**
This stretch project goes beyond the CCNA. It documents a site-to-site **IKEv2 IPsec VPN** between a Cisco router and a Juniper vSRX firewall, and **eBGP** from HQ to two simulated ISPs with controlled path preference.

## **Network Topology**
- **HQ:** Cisco router (CSR1000v or IOSv)
- **Branch:** Juniper vSRX firewall
- **ISP-A and ISP-B:** 2 simulated ISP routers
- **Platform:** EVE-NG

## **Project Objectives**
- Build an **IKEv2 IPsec** tunnel between two vendors
- Route traffic across the tunnel
- Configure **eBGP** to two ISPs
- Prefer ISP-A with local preference and filter what is accepted
- Document the interoperability problems and their fixes

---

## **1. Topology and Addressing**
1. **Draw the topology**
2. **Plan the addressing and AS numbers**

## Topology and Addressing - Visual Guide

<!-- screenshots -->


## **2. eBGP to Two ISPs**
1. **Configure the BGP sessions to both ISPs**
2. **Advertise only the HQ public prefix**
3. **Check the BGP tables**

## eBGP to Two ISPs - Visual Guide

<!-- screenshots -->


## **3. Path Preference and Filtering**
1. **Prefer ISP-A with local preference**
2. **Filter inbound routes to a default route**
3. **Test the failover to ISP-B**

## Path Preference and Filtering - Visual Guide

<!-- screenshots -->


## **4. IKEv2 IPsec Tunnel**
1. **Configure the IKEv2 proposal and policy on both sides**
2. **Configure the tunnel interfaces**
3. **Route the branch traffic through the tunnel**
4. **Verify the security associations**

## IKEv2 IPsec Tunnel - Visual Guide

<!-- screenshots -->


## **5. Interoperability Problems**
1. **Record each mismatch between the two vendors**
2. **Record the fix for each one**

## Interoperability Problems - Visual Guide

<!-- screenshots -->


## **Project Outcomes & Key Results**
- **Working Tunnel** – Traffic passing between HQ and the branch over IPsec
- **Path Control** – ISP-A preferred, ISP-B ready as a backup
- **Interoperability Notes** – The problems met between vendors and how they were solved

## **Potential Next Steps**
- **Add a third site with DMVPN**
- **Add BFD for faster failover**
- **Repeat with a Palo Alto firewall**

---

This project is part of my **Networking and Infrastructure portfolio**. For any inquiries, reach out via **[LinkedIn](https://www.linkedin.com/in/kimutai-fredrick/)**.

**_Built and documented by Fredrick Kimutai._**
