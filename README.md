# Advanced Intrusion Detection – SOC Case Study

A practical SOC investigation case study based on the **Advanced Intrusion Detection for SOC Analysts** guided project by Infosec.

## Project Overview
This project focuses on investigating a critical antivirus alert involving a malicious Microsoft Excel spreadsheet associated with TrickBot. The investigation covers malware identification, file behavior analysis, suspicious process execution, network activity, and SIEM-based threat hunting.

## Tools & Technologies
- **VirusTotal** – Malware identification and behavioral analysis
- **SIEM** – Hash-based investigation and endpoint scope assessment

## Investigation Tasks
- Analyzed the malicious file using its MD5 hash.
- Reviewed antivirus detection results.
- Examined VirusTotal sandbox behavior.
- Investigated suspicious process execution involving `rundll32.exe`.
- Reviewed external network communication.
- Performed a hash-based SIEM search for additional affected endpoints.
- Documented findings and remediation steps.

## Key Findings
- File type: Microsoft Excel Spreadsheet (`.xls`)
- Its other hash formats such as SHA-1, SHA-256, Vhash
- Malware classification: TrickBot-associated Trojan
- Process identified: `rundll32.exe`
- SIEM investigation: No additional endpoints identified using the file's MD5 hash.
- Confirmed investigation scope: One user workstation.

## Evidence
Screenshots and supporting investigation evidence are available in this repository.

## Remediation
1. Reset the user's network credentials.
2. Contact the impacted user.
3. Confirm device ownership.
4. Isolate the affected machine from the company network.
5. Wipe and reimage the machine, if possible.

## Certificate
Certificate of completion for the associated LinkedIn Learning course is included in this repository.
[View Certificate](Certificate/A Standalone Hands on practice SOC project by infosec)

## Final SOC Case Report
The complete investigation findings, IOCs, behavioral analysis,
SIEM investigation, and remediation steps are documented here.

[View SOC Case Report](report/soc-case-report.md)

## Disclaimer
This is a guided educational lab exercise. The scenario and investigation findings are based on the provided project materials, not a real-world incident response engagement.
