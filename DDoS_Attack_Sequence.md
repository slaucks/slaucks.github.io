```mermaid
sequenceDiagram
 actor Attacker 
 Attacker->>BotNet: BotNet Attack!
 BotNet->>Attacker: Ok
 BotNet->>Webserver: Spoofed SYN Packet
 BotNet->>Webserver: Spoofed SYN Packet
 BotNet->>Webserver: Spoofed SYN Packet
 BotNet->>Webserver: Spoofed SYN Packet
 BotNet->>Webserver: Spoofed SYN Packet
 Webserver->>Firewall: Help, I am being attacked by a DDoS attack
participant Firewall

```