# 🧠 Tusk Infostealer CTF – Challenge Solved

I just completed the **Tusk Infostealer** threat hunting challenge on CyberDefenders — using only a file hash, open-source intelligence, and some solid investigative techniques.

## 🚨 Scenario Recap
A blockchain developer was redirected to a fake DAO platform. Minutes later, their organization’s crypto wallets were drained. My task: uncover how the attack worked, identify IOCs, and track the attacker’s infrastructure.

## 🔍 What I Did

✅ Started with just an MD5/SHA256 hash — no sandbox, no dynamic tools  
✅ Used **Google Dorking** to pivot into Securelist’s threat report  
✅ Extracted and decoded the malware configuration (base64)  
✅ Identified the typosquatted domain (`tidyme[.]io`) spoofing peerme.io  
✅ Found second-stage payloads and archive password (`newfile2024`)  
✅ Pulled C2 IPs linked to **StealC**: `46[.]8[.]238[.]240`, `23[.]94[.]225[.]177`  
✅ Discovered clipper ETH wallet: `0xaf0362e215Ff4e004F30e785e822F7E20b99723A`  
✅ Mapped out fake AI translator domain: `voico[.]io` spoofing `Yous[.]ai`  
✅ Observed the attacker referred to victims as **"Mammoths"** in logs  

## 🔧 Tools Used
- Google (dorking)
- Securelist report
- ThreatFox
- Abuse.ch
- CyberChef
- strings & logic

## 🧠 What I Learned
- How to extract threat actor infrastructure from just a hash
- How clipboard hijackers silently steal crypto
- Importance of config decoding for deeper insight
- That you don’t need a lab to uncover real-world threats — just OSINT and mindset

## 🧑‍💻 Author
**Silas Binitie**  
GitHub: [slybdev](https://github.com/slybdev)  
LinkedIn: [silas-cybersec](https://www.linkedin.com/in/silas-cybersec)
