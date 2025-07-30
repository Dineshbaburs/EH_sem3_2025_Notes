# 🌐 Core Network Terms

**Date:** 2025-07-31  
**Prepared by:** Dinesh Babu R S  
**Reg no:** 2460360  
**Email:** dinesh.babu@btech.christuniversity.in  

---

## 🏠 NAT (Network Address Translation)

**Explanation:** NAT allows multiple devices in a local network to share one public IP address. It translates private IPs to a public IP when accessing the internet.

```
              [ Internet ]
                    |
         Public IP: 123.45.67.89
                    |
               ┌─────────┐
               │ Router  │
               └─────────┘
           ┌────┴────┬─────┬─────┐
           │         │     │     │
       ┌──────┐ ┌──────┐ ┌──────┐
       │Laptop│ │Phone │ │ Smart│
       │ .10  │ │ .11  │ │  TV  │
       └──────┘ └──────┘ └──────┘
   Private IPs: 192.168.1.X
```

---

## 🔍 ARP (Address Resolution Protocol)

**Explanation:** ARP is used to find the MAC address of a device when only its IP address is known.

```
Device A            Network            Device B
  |                   |                   |
  |-- Who has 192.168.1.20? --> Broadcast |
  |                   |                   |
  |<-- It's me! MAC: XX:XX:XX <--        |
  |                   |                   |
Now A can talk directly to B using MAC address
```

---

## 🆔 MAC Address

**Explanation:** A MAC address is a unique hardware ID for each device, used within local networks.

```
┌───────────────────────────┐
│   MAC Address:            │
│   AA:BB:CC:DD:EE:FF       │
├───────────────┬───────────┤
│ Manufacturer  │  Device ID│
│ Apple Inc.    │  Unique ID│
└───────────────┴───────────┘

Used for local device identification
```

---

## 🗘️ IPv4 - Internet Addressing

**Explanation:** IPv4 gives each device an IP address. It has about 4.3 billion possible addresses and is almost full.

```
IP Address: 192.168.1.10

Breakdown:
192    .   168    .   1    .   10
|         |        |        |
Network   Subnet   Host    Device
```

---

## 🚀 IPv6 - Next Generation Addressing

**Explanation:** IPv6 solves the IPv4 address shortage. It offers automatic setup and much larger address space.

```
IPv6: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

More space:
- IPv4: 4.3 billion addresses
- IPv6: 340 undecillion addresses
```

---

## 🔄 How They Work Together

**Example: Complete Data Journey**

```
1. User opens browser and types a URL
2. DNS resolves the domain to an IP address
3. ARP finds router’s MAC address
4. Device sends request using NAT and router’s public IP
5. Server responds and router forwards to the right device
```

---

## ⚠️ Common Network Attacks

```
• MAC Spoofing: Impersonate a trusted device using a fake MAC
• ARP Poisoning: Send false ARP replies to intercept data
• IP Scanning: Probe network for active IPs
• NAT Confusion: Misrouting due to incorrect translations
```

---

## ✅ Summary

- 🆔 **MAC:** Unique device identifier  
- 📞 **ARP:** Matches IP with MAC  
- 📬 **IPv4:** Limited internet address system  
- 🌌 **IPv6:** Vast future-ready address system  
- 🔄 **NAT:** Shares one public IP among private devices  

📘 Knowing these basics helps you understand how internet connections work and how devices communicate securely.
