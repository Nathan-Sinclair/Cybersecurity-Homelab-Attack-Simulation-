# Cybersecurity-Homelab-Attack-Simulation-

## Purpose:
This project simulates a full end‑to‑end cyberattack against a purpose‑built homelab to validate SIEM detections and response. It demonstrates recon, initial access, lateral movement, privilege escalation, data exfiltration, and persistence, while showing how Wazuh alerts and supports investigation — for controlled, educational use only.

## Implementation:
- Added Kali attacker VM on the lab NAT network.
- Reconnaissance with nmap; identified SSH, MailHog, WinRM, RDP.
- Initial access via SSH brute (Hydra) and credential capture from MailHog phishing.
- Lateral movement and WinRM takeover (NetExec → Evil‑WinRM); RDP to Domain Controller.
- Data exfiltration with scp and persistence via a scheduled PowerShell reverse shell.
- Validated detections and investigated alerts in Wazuh; documented snapshots and commands for reproducibility.

## Skills Demonstrated:
- **VM & Lab Setup**: Provisioned and managed Kali, Windows, and Linux VMs with NAT networking and snapshots.
- **Offensive Security**: Performed reconnaissance, SSH brute-force, phishing, lateral movement, and privilege escalation.
- **Persistence & Exfiltration**: Created admin accounts, scheduled reverse shells, and securely exfiltrated sensitive files.
- **SIEM & Monitoring**: Validated alerts and investigated events in Wazuh.
- **Scripting & Automation**: Used Python, Bash, and PowerShell for attack simulation and automation.
- **AD & Windows Admin**: Managed users, groups, and RDP/WinRM access in lab domain.

## Prerequisites & Dependencies:
Refer to Cybersecurity-Homelab-Building-The-Environment readme.

## Documentation/Step By Step Guide:
Full step-by-step setup and configuration instructions are provided in the accompanying PDF file.
[Here Is The Link](Cybersecurity%20Homelab%20Attack%20Simulation%20Documentation.pdf)

## Credits:

- Developed by Nathan Sinclair, inspired by Grant Collins’ Build a Cybersecurity Homelab: Enterprise 101 (https://projectsecurity.teachable.com/p/build-a-cybersecurity-homelab-a-practical-guide-to-offense-defense-enterprise-101). Special thanks to Grant Collins for creating such a valuable learning resource. 

- Tools used include Wazuh, Kali Linux, Security Onion, MailHog, VirtualBox, and Windows/Ubuntu OSs. 

- Documentation and content suggestions assisted by ChatGPT and other large language models (LLMs), with thanks to the open-source communities behind the tools. 
