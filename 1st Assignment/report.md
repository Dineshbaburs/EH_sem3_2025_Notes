# Network Fundamentals Report

**Date:** 2025-07-31  
**Prepared by:** Dinesh Babu R S  
**Reg no:** 2460360  
**Email:** dinesh.babu@btech.christuniversity.in  
**Subject:** Core Network Terms

---

## NAT (Network Address Translation)

**Explanation:** NAT allows multiple devices in a local network to share one public IP address. It translates private IPs to a public IP when accessing the internet.

```
Your Home Network:
┌────────────┐    ┌───────────┐    ┌────────────┐
│ Laptop     │    │ Phone     │    │ TV         │
│192.168.1.10│    │192.168.1.11│   │192.168.1.12│
└────────────┘    └───────────┘    └────────────┘
        │               │                │
        └──────────────┼────────────────┘
                        │
                 ┌────────────┐
                 │ Router     │  -> Public IP: 123.45.67.89
                 └────────────┘
                        │
                     Internet
```

---

## ARP (Address Resolution Protocol)

**Explanation:** ARP is used to find the MAC address of a device when only its IP address is known.

```
Computer A wants to send data to Computer B:
- A sends ARP request: "Who has IP 192.168.1.20?"
- B replies with its MAC address.
```

---

## MAC Address

**Explanation:** A MAC address is a unique hardware ID for each device, used within local networks.

```
MAC Example: AA:BB:CC:DD:EE:FF
- First half: Manufacturer ID
- Second half: Device-specific ID
```

---

## IPv4 - Internet Addressing

**Explanation:** IPv4 gives each device an IP address. It has about 4.3 billion possible addresses and is almost full.

```
Example: 192.168.1.10
Structure: Network.Subnet.Device
```

---

## IPv6 - Next Generation Addressing

**Explanation:** IPv6 solves the IPv4 address shortage. It offers automatic setup and much larger address space.

```
Example: 2001:db8::1
Total Addresses: 340 undecillion
```

---

## How They Work Together

**Example:**
1. You open a website.
2. Your computer asks for the IP address.
3. ARP finds your router’s MAC.
4. NAT changes your IP to the public one.
5. Internet communication begins.

---

## Common Network Attacks

- **MAC Spoofing:** Pretending to be another device on the network.
- **ARP Poisoning:** Giving false MAC address info to mislead devices.
- **IP Scanning:** Looking for active IP addresses.
- **NAT Confusion:** Packets being misrouted due to multiple translations.

---

## Summary

- **MAC:** Unique device identifier  
- **ARP:** Matches IP with MAC  
- **IPv4:** Limited internet address system  
- **IPv6:** Vast future-ready address system  
- **NAT:** Shares one public IP among private devices  

Knowing these basics helps you understand how internet connections work and how devices communicate securely.
