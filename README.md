# INF249 – Padding Oracle Lab (MA3)

This project is a practical security assignment from  
**INF249 – Network Security (University of Bergen).**

## Scenario
The goal was to decrypt a block of ciphertext using a **live padding oracle**
running on a machine inside a simulated internal network. :contentReference[oaicite:0]{index=0}

A key assumption was that one user’s password had mistakenly been set to **"test"**.

## What I did (high-level)

- **Network discovery**
  - Identified all active IP addresses in the local lab network.

- **Initial access**
  - Leveraged the known weak password to gain a foothold on the system.

- **Privilege escalation**
  - Found and exploited a local privilege escalation vector to access useful data.

- **Reach the oracle**
  - Navigated the internal network to locate and access the machine hosting the padding oracle.

- **Padding oracle attack**
  - Interacted with the oracle to iteratively decrypt a block of ciphertext encrypted in CBC mode.
  - Successfully recovered the correct plaintext/ciphertext pair.

## Concepts demonstrated
- CBC mode and padding
- Padding oracle vulnerabilities  
- Network enumeration  
- Lateral movement  
- Privilege escalation in Linux  

## Tools
- Linux CLI  
- SSH  
- Network scanning utilities  
- Custom interaction with the padding oracle  

## Documentation
Full report: `report/INF249_MA3_padding_oracle.pdf`
