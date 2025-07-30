# 🌐 Core Network Terms - Report

> 💼 A beginner-friendly guide to understanding the hidden language of the internet.

**👤 Prepared by:** Dinesh Babu R S  \
**📅 Date:** 2025-07-31  \
**🆔 Reg No:** 2460360  \
**📧 Email:** [dinesh.babu@btech.christuniversity.in](mailto\:dinesh.babu@btech.christuniversity.in)

---

## 🧭 NAT (Network Address Translation)

**📘 What it is:** A technique that lets many devices share one public IP address.\
**🔐 Why it matters:** It keeps your internal network secure and conserves public IP addresses.

```
              [ 🌐 Internet ]
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

📶 NAT is essential for enabling multiple devices to connect to the internet securely using one IP address.

---

## 🔍 ARP (Address Resolution Protocol)

**📘 What it is:** A protocol used to find a device’s MAC address when its IP address is known.\
**🔄 Why it matters:** Enables direct device-to-device communication in a local network.

```
Device A            Network            Device B
    |                   |                   |
    |-- Who has 192.168.1.20? --> Broadcast |
    |                   |                   |
    |<-- It's me! MAC: XX:XX:XX <--        |
    |                   |                   |
Now A can talk directly to B using MAC address
```

📡 ARP ensures seamless data delivery by mapping IP addresses to physical hardware addresses.

---

## 🆔 MAC Address

**📘 What it is:** A globally unique identifier assigned to each device’s network interface card (NIC).\
**🎯 Why it matters:** Acts as a digital signature for devices within a local network.

```
┌─────────────────────────────┐
│   MAC Address:              │
│   AA:BB:CC:DD:EE:FF         │
├────────────────┬───────────┤
│ Manufacturer   │ Device ID │
│ Apple Inc.     │ Unique ID │
└────────────────┴───────────┘
```

🔎 Useful for authentication, filtering, and tracking device-specific activities.

---

## 🌐 IPv4 - Internet Addressing

**📘 What it is:** A 32-bit addressing system currently used by most internet-connected devices.\
**📉 Why it matters:** Its limited space (4.3 billion addresses) is running out.

```
IP Address: 192.168.1.10

Breakdown:
192    .   168    .   1    .   10
|         |        |        |
Network   Subnet   Host    Device
```

🔢 IPv4 is familiar and widely deployed, but constrained in scale.

---

## 🚀 IPv6 - Next Generation Addressing

**📘 What it is:** A 128-bit addressing scheme designed to replace IPv4.\
**🌍 Why it matters:** Supports virtually unlimited unique IPs and simplifies address configuration.

```
IPv6: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

IPv4: 4.3 billion  vs  IPv6: 340 undecillion
```

⚙️ IPv6 ensures future readiness, enhanced security, and efficient routing.

---

## 🔄 How They Work Together

**📘 Example Scenario:** Accessing a website from a device within a home network:

```
1. You type a URL into your browser.
2. DNS resolves the domain to an IP address.
3. ARP finds the MAC address of your default gateway (router).
4. NAT converts your private IP to a public one.
5. The server responds and the router delivers the content back to your device.
```

🔁 Collaboration among these protocols ensures successful communication over networks.

---

## 🛡️ Common Network Attacks

**⚠️ Be cautious of these threats:**

```
• MAC Spoofing: Masquerading as another device to gain unauthorized access
• ARP Poisoning: Injecting false MAC info to intercept network traffic
• IP Scanning: Searching for vulnerable hosts on the network
• NAT Confusion: Exploiting address translation inconsistencies
```

🧱 Employ strong firewall rules, MAC filtering, and encryption to mitigate risks.

---

## 📌 Recap at a Glance

- 🆔 **MAC Address:** Hardware identity of a device
- 📡 **ARP:** Resolves IP addresses to MAC addresses within local networks
- 🌐 **IPv4:** Legacy internet protocol still in wide use
- 🌍 **IPv6:** Modern, scalable addressing for future networks
- 🔁 **NAT:** Connects multiple local devices to the internet securely via one public IP

📖 **Takeaway:** Mastering these concepts forms the foundation of computer networking and improves both problem-solving and cybersecurity awareness.
