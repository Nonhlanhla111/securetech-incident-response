# SecureTech Solutions: Incident Response Report (SEC-IR-2026-001)

Cybersecurity practical assessment: investigation of a suspected malware infection and unusual network
activity on a Windows workstation, carried out in an authorised lab using free tools.

## Contents
- `report/`: final incident response report (Word and PDF)
- `evidence/day1/`: Microsoft Defender and EICAR detection screenshots
- `evidence/day2/`: Wireshark and Event Viewer screenshots (account name redacted)

## Summary
| Area | Result |
|---|---|
| Antivirus | Defender detected and removed the EICAR test file (Virus:DOS/EICAR_Test_File) |
| Network | ICMP, DNS, TCP and TLS traffic matched expected activity; no unexpected destinations seen |
| Windows logs | 547 failed logons (4625) were all local; no remote logons or guessing patterns |
| Conclusion | Insufficient evidence of a genuine attack; control improvements recommended |

## Tools
Microsoft Defender, Windows Firewall, EICAR test file, Wireshark/Npcap, Event Viewer.

## Notes
- This is a simulation. Only the harmless EICAR test string was used; no real malware.
- Packet captures (`.pcapng`) are excluded on purpose because they contain internal addresses and background traffic.
