Phishing Email Investigation

A hands-on cybersecurity lab focused on identifying and investigating phishing emails using email header analysis, email authentication checks, URL analysis, IOC extraction, and incident reporting.

## Project Overview

This project demonstrates a SOC-style phishing email investigation process using two controlled and synthetic phishing cases.

The investigations focus on identifying suspicious sender information, analyzing email authentication results, examining email headers, extracting Indicators of Compromise (IOCs), and documenting the investigation findings.

## Cases Investigated

### Case 01 – PayPal Impersonation Phishing

Investigation of a simulated PayPal impersonation phishing email containing:

* Look-alike sender domain
* Mismatched Reply-To address
* SPF failure
* Missing DKIM signature
* DMARC failure
* Suspicious verification URLs
* Extracted phishing indicators and IOCs

### Case 02 – Microsoft 365 Credential Phishing

Investigation of a simulated Microsoft 365 credential phishing email containing:

* Look-alike Microsoft domain
* Mismatched Reply-To domain
* SPF failure
* Missing DKIM signature
* DMARC failure
* Urgency-based password expiration message
* Suspicious account verification URL
* Extracted phishing indicators and IOCs

## Investigation Methodology

The following workflow was used during the investigations:

1. Email Header Analysis
2. Sender and Reply-To Analysis
3. SPF, DKIM and DMARC Verification
4. Source IP Identification
5. Suspicious URL Analysis
6. IOC Extraction
7. Social Engineering Analysis
8. MITRE ATT&CK Mapping
9. Risk Assessment
10. Incident Reporting

## Tools & Technologies

* Email Header Analysis
* SPF / DKIM / DMARC
* VirusTotal
* MITRE ATT&CK
* IOC Analysis
* Microsoft Word
* Windows

## Project Structure

```text
phishing-email-investigation/
│
├── README.md
│
├── Case-01_PayPal_Impersonation_Phishing/
│   ├── Evidence_01/
│   ├── Report_01/
│   ├── IOCs_01/
│   ├── Analysis_Notes_01.txt
│   └── screenshots_01/
│
└── Case-02_Microsoft365_Credential_Phishing/
    ├── Evidence_02/
    ├── Report_02/
    ├── IOCs_02/
    ├── Analysis_notes_Case-02.txt
    └── Screenshots_02/
```

## Key Findings

Both simulated phishing cases contained multiple indicators associated with phishing activity, including look-alike domains, mismatched sender information, failed email authentication, suspicious URLs, and social-engineering techniques.

The investigations resulted in a **High Risk / Phishing** assessment for both cases.

## MITRE ATT&CK

The phishing scenarios were mapped to:

* **T1566 – Phishing**
* **T1566.002 – Phishing: Spearphishing Link**

## Evidence

The repository contains:

* Synthetic `.eml` email evidence
* Investigation reports
* IOC files
* Analysis notes
* Investigation screenshots

## Disclaimer

This project is intended for cybersecurity education and portfolio demonstration.

All domains ending in `.test` and documentation IP addresses used in the lab are synthetic/test artifacts. No real malicious activity is attributed to these indicators.

## Skills Demonstrated

* Phishing Detection
* Email Header Analysis
* Email Authentication Analysis
* IOC Extraction
* Threat Intelligence Analysis
* Social Engineering Detection
* MITRE ATT&CK Mapping
* SOC Investigation & Documentation
* Incident Reporting
