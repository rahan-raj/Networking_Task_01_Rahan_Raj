# Networking_Task_01_Rahan_Raj
The purpose of this task is to understand the basic components of a network and identify the network configuration of our own device.

---

**Intern:** Rahan Raj K R 

**Date:** June 2026  
**Organization:** White Band Associates  

---

## Part A: Network Information

| Detail | Value |
|---|---|
| Hostname | DESKTOP-L3P3HQF |
| IPv4 Address | 192.168.1.9 |
| MAC Address | 70-77-81-2B-36-05 |
| Default Gateway | 192.168.1.1 |
| DNS Server | 8.8.8.8 |

> Screenshots of `ipconfig` output are in the `/Screenshots` folder.

---

## Part B: Basic Networking Concepts

### What is an IP Address?
 Think of it like your home address, but for your device on a network. It tells other devices where to send data. Ex. 192.168.1.9

### What is a MAC Address?
A permanent, unique ID created into your network card by the manufacturer. Unlike an IP address, it never changes. Ex. 00:1b:63:84:45:e6

### What is a Default Gateway?
 It is known as the ”exit point”or "front door" for your device when you need to connect with another network. When you want to reach the internet, your data first goes to the gateway (usually your router).

### What is DNS?
 A phonebook for the internet. Instead of remembering that Google is at 142.250.74.46, you just type google.com and DNS translates it to the right IP address.

### Difference between Public IP and Private IP

Public IP (Internet Address)
- Given by your Internet Service Provider (ISP) .
- Used when you connect to websites like Google, YouTube, etc. 
- It is visible to the outside world.
  
Private IP(Local Network Address)
- Assigned by your router 
- Used only inside your home/office WiFi 
- Not visible on the internet
---

## Part C: Network Diagram

```
          [ Internet ]
               |
        [ Router / WiFi ]
          192.168.1.1
               |
        [ Your Device ]
          192.168.1.9
```

> A detailed diagram image is included as `Network Diagram.png` in this repository.

---

## Part D: Network Connectivity Test

### Commands run (Windows)

```
ipconfig 
ping google.com
tracert google.com
```

### Results

**1. Was the ping successful?**  
Yes. I received 4 replies from google.com with 0% packet loss. Average response time was approximately 151 ms.

**2. How many hops were shown in tracert?**  
The traceroute showed 30 hops to reach google.com.

**3. What is the purpose of traceroute?**  
Traceroute maps the exact path that data takes from my device to a destination, showing every router it passes through and the time each hop takes. It is useful for diagnosing where slowdowns or failures are occurring in a network connection.

> Screenshots of all command outputs are in the `/command outputs` folder.  


---

## What I Learned

- How to find my device's network configuration using `ipconfig`
- The difference between a private IP (local network) and a public IP (internet address)
- How DNS translates domain names into IP addresses
- How data travels in hops across the internet, as shown by traceroute
- How to document and organise technical findings in a GitHub repository

---

## Tools Used

- Windows Command Prompt (`ipconfig`, `ping`, `tracert`)
- Draw.io for the network diagram
- GitHub for version control and submission
