# Cybersecurity-Tips
The 3 Protocols Every Cybersecurity Engineer Must Truly Understand (DHCP, ARP, DNS)

Most beginners think cybersecurity starts with firewalls, SIEM, or hacking tools.

It doesn’t.

Cybersecurity starts the moment a device joins a network and tries to answer three questions:

Who am I?
Who is around me?
How do I find others?

Those answers come from DHCP, ARP, and DNS — the real foundation of identity and discovery on every network.

🧭 DHCP — “Who am I?” (DORA)

When a device connects, it has no IP address. It literally shouts:

“Is there any DHCP server out there?”

Through Discover → Offer → Request → Acknowledge, the device becomes someone on the network.

🔐 Security insight:

Rogue DHCP = Man-in-the-Middle

DHCP logs tell you who had what IP and when

Critical during investigations

🔗 ARP — “Who has this IP?”

IP is Layer 3. Communication on a LAN happens with MAC addresses (Layer 2).

So the device asks:

“Who has 192.168.1.1?”

The owner replies with its MAC address. Now they can talk.

🔐 Security insight:

ARP spoofing & poisoning power many MITM attacks

Tools like Ettercap and Bettercap abuse this

Understanding ARP = understanding silent interception

🌍 DNS — “How do I find others?”

Humans remember names, not IPs.

Your device asks a resolver for the IP of a domain, which walks:
Root → TLD → Authoritative server and returns the answer.

🔐 Security insight:

DNS is the backbone of malware communication

DNS tunneling, C2 beacons, phishing, DGA

You can detect malware just by watching DNS queries

Why This Matters in SOC & Threat Hunting

Every investigation often follows this path:

Suspicious domain → DNS log → IP → DHCP lease → MAC → Device → User

No fancy tool. Just protocol understanding.

This is the difference between:
Someone who memorises tools and someone who thinks like a cybersecurity engineer.

Final Thought

Before SIEM.
Before EDR.
Before firewalls.

There is identity and discovery.

DHCP gives identity.
ARP enables local communication.
DNS connects to the world.

Master these three, and you begin to understand the language of networks — and cybersecurity is simply the art of listening to that language.

#CyberSecurity #SOC #Networking #ThreatHunting #BlueTeam #DHCP #ARP #DNS #CyberTraining # CyberNovaAcademy

[ping in Network.Diagnosis] https://github.com/hephzibahdaniel/Cybersecurity-Tips/blob/main/Ping%20in%20Network%20Diagnostics%3A%20Practical%20Applications%20for%20Cybersecurity%20Professionals
