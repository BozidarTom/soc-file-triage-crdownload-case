# SOC File Triage Case – Suspicious .crdownload File

## Overview
This project documents a real-world SOC-style investigation of a suspicious file found on a user endpoint.
The file had a `.crdownload` extension, raising concerns about potential malware.

The goal of this case study is to demonstrate SOC L1 file triage methodology, decision-making, and documentation.

---

## Incident Summary
- Alert Type: Suspicious File on Endpoint
- File Name: Unconfirmed 879939.crdownload
- User Concern: Possible malware
- Environment: Windows endpoint, Google Chrome browser
- Initial Risk: Medium (unknown downloaded file)

---

## Analysis Steps

### 1. File Extension Review
- `.crdownload` indicates an incomplete Chrome download

### 2. File Header & Type Identification
- ZIP header (`PK`) identified
- File recognized as Microsoft Word document (.docx)

### 3. Archive Structure Inspection
- Standard Word document structure
- No executable content found

### 4. Macro & Script Analysis
- No macros detected
- No embedded scripts

---

## Findings
- Incomplete Word document
- No malicious indicators
- No macros or executables

---

## Conclusion
- Verdict: False Positive
- Risk Level: Low
- Recommended action: Delete file
- Escalation: Not required

---

## SOC Analyst Takeaways
- Not all unusual files are malicious
- File type verification is critical
- Proper triage prevents false escalation
