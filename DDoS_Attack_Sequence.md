```mermaid
sequenceDiagram
 actor Attacker 
 Attacker->>BotNet: BotNet Attack!
 destroy Attacker
 BotNet->>Attacker: Ok
 BotNet->>Webserver: Spoofed SYN Packet
 BotNet->>Webserver: Spoofed SYN Packet
 BotNet->>Webserver: Spoofed SYN Packet
 BotNet->>Webserver: Spoofed SYN Packet
 BotNet->>Webserver: Spoofed SYN Packet
 Webserver->>Firewall: Help, I am being attacked by a DDoS attack
 Firewall->>Webserver: I will enable rate limiting to slow the rate of requests
 destroy Webserver
 Firewall->>BotNet: I have enabled traffic analysis and have discovered where these requests are coming from 
 Firewall->>BotNet: I have enabled IP blocking on thes addresses
participant Firewall

```