# SecureTech Solutions: Incident Response Report (SEC-IR-2026-001)

Cybersecurity practical assessment: investigation of a suspected malware infection and unusual
network activity on a Windows workstation, carried out in an authorised lab using free tools.

## Assessment brief
As a junior security analyst at SecureTech Solutions (a fictional company), I was asked to
investigate a possible malware infection on a Windows workstation, gather digital evidence,
identify security risks and recommend protective measures. The incident was simulated using
free software and a harmless test file; no real malware was used. The work ran over three days.

| Day | Activity | What was asked | Where it appears in the report |
|---|---|---|---|
| 1 | A: Workstation security assessment | Check antivirus, real-time protection and firewall status; run a quick scan | Section 5.1 |
| 1 | B: Simulated malware detection | Download the EICAR test file with antivirus on; record how Defender responds and the Protection history entry | Section 5.2 |
| 1 | C: Initial findings | Summarise what was observed and how the organisation should respond to a similar alert | Sections 1 and 6 |
| 2 | A: Network traffic capture | Capture traffic in Wireshark while running ping, nslookup and a website visit; analyse ICMP, DNS, TCP and TLS packets | Section 5.3 |
| 2 | B: Windows security investigation | Review Security log events 4624 (successful logon) and 4625 (failed logon) in Event Viewer | Section 5.4 |
| 2 | C: Incident analysis | Decide whether the evidence shows a genuine attack | Section 5.5 |
| 3 | A: Incident response plan | Verify the alert, preserve evidence, decide on isolation, remove threats, restore operations | Section 6 |
| 3 | B: Final technical report | Combine scenario, tools, method, screenshots, findings, controls and lessons learned | The whole report |

## Contents
- `report/`: final incident response report

  📄 **[Secure Tech Incident Report](report/SecureTech__Incident_Report.pdf)**

This is a sanitised copy: the computer name, internal IP addresses and account name are replaced or
blacked out. Raw screenshots and packet captures are not included.

## Summary of results
| Area | Result |
|---|---|
| Antivirus | Defender detected and removed the EICAR test file (Virus:DOS/EICAR_Test_File) |
| Network | ICMP, DNS, TCP and TLS traffic matched expected activity; no unexpected destinations seen |
| Windows logs | 547 failed logons (4625) were all local; no remote logons or guessing patterns |
| Conclusion | Insufficient evidence of a genuine attack; control improvements recommended |

## Tools
Microsoft Defender, Windows Firewall, EICAR test file, Wireshark/Npcap, Event Viewer.
