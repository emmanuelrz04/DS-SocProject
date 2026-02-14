Attack Chain Analysis – Phishing Scenario

This project applies the Cyber Kill Chain model to analyze a phishing-based attack from a SOC (Security Operations Center) perspective. The goal is to understand how the attack progresses and at which stages defensive monitoring can identify suspicious activity.

1. Reconnaissance
The attacker gathers publicly available information about the target, such as email addresses, organizational structure, and service providers. This information may be obtained from social media, data leaks, or automated harvesting tools.

2. Weaponization
The attacker prepares the phishing artifact. In this scenario, this includes the creation of:
A spoofed email template
A fake login page or malicious attachment
Embedded tracking mechanisms (e.g., remote content)

3. Delivery
The phishing email is sent to the victim. Indicators at this stage may include:
Suspicious or recently registered domains
Email spoofing attempts
Inconsistent sender addresses
Encoded attachments (e.g., base64 PDF files)
From a SOC perspective, email gateway logs and domain reputation checks are critical at this stage.

4. Exploitation
The victim interacts with the malicious content by:
Clicking on a link
Downloading an attachment
Entering credentials on a fake website
Detection opportunities include:
Abnormal login attempts
Access from unfamiliar IP addresses
Unusual login times

5. Installation
If malware is involved, it may be installed on the victim’s system. Monitoring endpoint logs and suspicious process execution becomes essential.
6. Command and Control (C2)
The compromised system may communicate with an external malicious server. SOC teams monitor outbound connections to unknown domains or flagged IP addresses.

7. Actions on Objectives
The attacker achieves their objective, such as credential theft, financial fraud, or data exfiltration.
SOC Detection Focus in This Project
This project emphasizes detection in the Delivery and Exploitation stages by simulating:
Suspicious domain validation
Detection of spoofed sender addresses
Abnormal login pattern analysis
Identification of encoded attachments
The objective is to demonstrate how structured monitoring and rule-based analysis can reduce phishing-related risk within an organization.
