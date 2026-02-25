https://tryhackme.com/room/cyberkillchainzmt?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=copy&sharerId=692d67d949c2314779ad896d

Cyber Kill Chain – TryHackMe Write-up

Date: Feb.14,2026

This room focused on understanding the Cyber Kill Chain framework and identifying each phase based on given scenarios. The challenge was more about recognizing definitions and matching activities to the correct stage rather than technical exploitation.

The Cyber Kill Chain was developed by Lockheed Martin. It describes the stages of a cyber attack from planning to execution.

The seven stages covered in the room are:

1) Reconnaissance  
This is the information-gathering stage. The attacker collects data about the target such as email addresses, employee names, domains, IP ranges, or technologies used. This is usually passive and can involve OSINT techniques.

2) Weaponization  
In this phase, the attacker creates a malicious payload. This could be malware combined with an exploit, such as a malicious document or executable file prepared for delivery.

3) Delivery  
The attacker sends the weaponized payload to the victim. Common methods include phishing emails, malicious attachments, infected USB drives, or compromised websites.

4) Exploitation  
This is when the malicious code is triggered. A vulnerability is exploited to execute the attacker’s code on the victim’s system.

5) Installation  
After successful exploitation, the attacker installs malware or a backdoor to maintain access to the system.

6) Command and Control (C2)  
The infected system communicates with the attacker’s server. This allows remote control, data exfiltration, or additional instructions.

7) Actions on Objectives  
This is the final stage where the attacker achieves their goal. This may include data theft, privilege escalation, lateral movement, or system disruption.

Throughout the room, the questions required identifying which stage a specific activity belonged to. The key to solving the room was understanding the definitions of each phase and carefully reading the scenario descriptions.

Key Takeaways:
- The Cyber Kill Chain helps break down attacks into structured stages.
- Many attacks can be detected or stopped if identified early in the chain.
- Defensive strategies improve when you understand how attackers operate step by step.

This room strengthened my understanding of attack progression and reinforced how important early detection is in cybersecurity.
