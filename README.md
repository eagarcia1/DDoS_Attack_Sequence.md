# DDoS_Attack_Sequence.md

```mermaid
sequenceDiagram
    participant Attacker
    participant BotNet
    participant WebServer
    participant Firewall

    Attacker->>BotNet: Command to initiate attack
    BotNet->>WebServer: Flood requests
    BotNet->>Firewall: Attempt to bypass
    Firewall->>WebServer: Block suspicious traffic
    WebServer->>Firewall: Respond with status
    Firewall->>BotNet: Drop malicious traffic
    WebServer->>BotNet: Slow response due to overload

```
    
Attacker will send signal to bots in a loop
spread command to bots end
bots now activated for attack
WebServer communicates to Firewall
Detect abnormal traffic
Firewall acts based on traffic patterns
Traffic exceeds limit
Blacklist offending IPs
Allow safe traffic
