# Networking Fundamentals — Week 1

## Day 1
- Learned the basics of how networks and the internet work
- Learned the difference between IP addresses and MAC addresses:
  - IP address — logical address used for routing traffic across networks
  - MAC address — physical/hardware address unique to a network interface
- Learned how `PING` works using ICMP (Internet Control Message Protocol)
  to test whether a device is reachable on the network
- Completed the "What is Networking" room on TryHackMe ✅
  (5 tasks completed, 80 points)

## Day 2
- Completed the "Intro to LAN" room on TryHackMe ✅ (5 tasks, 152 points, streak: 2)
- Learned LAN (Local Area Network) fundamentals:
  - Network topologies — different ways devices can be physically/logically
    arranged and connected (e.g. star, bus, ring)
  - Switches — connect devices within the same LAN, forward traffic based
    on MAC addresses
  - Routers — connect different networks together and direct traffic
    between them
  - ARP (Address Resolution Protocol) — resolves an IP address to a MAC
    address on the local network
  - DHCP (Dynamic Host Configuration Protocol) — automatically assigns IP
    addresses to devices, using a request/reply process between the
    device and the DHCP server

## Day 3 (self-study — PowerCert / NetworkChuck)
- Learned the OSI Model — the 7-layer framework for how data moves across
  a network:
  1. Physical — raw transmission of bits over cables/wireless
  2. Data Link — handles MAC addresses and framing (e.g. switches)
  3. Network — handles IP addressing and routing (e.g. routers)
  4. Transport — handles reliable delivery, using TCP or UDP
  5. Session — manages connections/sessions between devices
  6. Presentation — handles data formatting, encryption/decryption
  7. Application — where actual applications interact with the network
     (HTTP, DNS, etc.)
- Learned the TCP/IP Model — the simplified, practical 4-layer model used
  in real-world networking:
  1. Network Access — combines OSI's Physical + Data Link layers
  2. Internet — handles IP addressing and routing (maps to OSI's Network layer)
  3. Transport — handles TCP/UDP, same role as OSI's Transport layer
  4. Application — combines OSI's Session, Presentation, and Application layers
- Key takeaway: OSI is the theoretical/teaching model, TCP/IP is the model
  actually used on real networks — but both describe the same underlying
  process of getting data from one device to another

## Day 4
- Completed the "OSI Model" room on TryHackMe ✅ (10 tasks, 224 points, streak: 1)
- Learned the OSI Model — the 7-layer framework for how data moves across
  a network:
  1. Physical — raw transmission of bits over cables/wireless
  2. Data Link — handles MAC addresses and framing (e.g. switches)
  3. Network — handles IP addressing and routing (e.g. routers)
  4. Transport — handles reliable delivery, using TCP or UDP
  5. Session — manages connections/sessions between devices
  6. Presentation — handles data formatting, encryption/decryption
  7. Application — where actual applications interact with the network
     (HTTP, DNS, etc.)

## Day 5
- Completed the "Packets & Frames" room on TryHackMe ✅ (6 tasks, 80 points, streak: 2)
- Learned how data is broken down and transmitted across a network:
  - Packets — data is split into smaller units at the Network layer, each
    packet carrying source/destination IP addresses
  - Frames — packets get wrapped into frames at the Data Link layer,
    adding source/destination MAC addresses for local delivery
  - Encapsulation — as data moves down the OSI layers, each layer adds
    its own header (and sometimes trailer) around the data — this whole
    process is called encapsulation, and it's reversed (de-encapsulation)
    on the receiving end

## Day 6
- Completed the "Extending Your Network" room on TryHackMe ✅ (6 tasks, 88 points, streak: 2)
- Learned how a LAN connects safely to the internet:
  - NAT (Network Address Translation) — translates private internal IP
    addresses to a single public IP so multiple devices on a LAN can
    share one internet connection
  - Firewalls — filter incoming/outgoing traffic based on rules, deciding
    what's allowed in and out of a network
  - Why these matter together: NAT hides internal network structure from
    the outside world, while firewalls control what traffic is permitted
    to cross that boundary
