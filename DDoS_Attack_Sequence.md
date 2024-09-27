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
 participant Firewall

```