# 📧 Phishing Email Analysis – Fake ZipRecruiter Job Offer

This project documents the analysis of a **simulated phishing email** mimicking a job offer from ZipRecruiter. It was analyzed as part of a cybersecurity task focused on identifying phishing techniques, malware risks, and social engineering.

---

## 📨 Email Summary

- **From**: `noreply-zip-recruiter@authwebmail.com`
- **To**: `amish.ck@mybusiness.com`
- **Subject**: Congratulations! Selected for Global Expansion Officer at PaySphere
- **Attachment**: `CanIPhish-Word-Attachment.docx`

---

## 🛠 Objective

Analyze the phishing email to:
- Detect spoofed sender information
- Identify signs of phishing or malware
- Evaluate social engineering techniques
- Document suspicious attachments or content

---

![t2-1](https://github.com/Amish-C-K/Elevate-Labs--task2/blob/main/images/t2-1.png)

![t2-2](https://github.com/Amish-C-K/Elevate-Labs--task2/blob/main/images/t2-2.png)

---

## 🔍 Phishing Indicators

| # | Indicator | Details |
|--|-----------|---------|
| 1 | 🕵️ Spoofed Domain | Email sent from `authwebmail.com`, not ZipRecruiter’s domain. |
| 2 | 🎯 Unrealistic Offer | Salary claim of $275k–$325k is unusually high and unsolicited. |
| 3 | 📎 Malicious Attachment | `.docx` file triggers "Enable Editing" warning – used in macro malware. |
| 4 | ⚠️ Urgency | Pushes recipient to respond quickly (“intro call this week”). |
| 5 | 🧷 Broken Content | Word doc contains missing image links — a known phishing technique. |
| 6 | 🔗 No Verifiable Links | No official site URLs included; cannot confirm legitimacy. |
| 7 | 💬 Generic Language | Mentions LinkedIn with no personal detail — clearly templated. |

---

## 📎 Attachment Behavior

**File**: `CanIPhish-Word-Attachment.docx`  
**Findings**:
- Opened in Protected View
- Missing image references
- Requests user to "Enable Editing"
- ⚠️ **Scanned with VirusTotal**: Marked as **malicious and phishing**

---

## 🧰 Recommended Tools (for Real-World Analysis)

Although this was a **training simulation**, the following tools are recommended for analyzing real phishing emails:

### 📬 Email Header Analysis
- [MxToolbox Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- [Google Admin Toolbox – Message Header](https://toolbox.googleapps.com/apps/messageheader/)

### 🔗 Suspicious URL Analysis
- [VirusTotal – URL Scanner](https://www.virustotal.com/gui/home/url)
- [URLScan.io](https://urlscan.io/)

### 📎 Attachment (DOCX/PDF) Analysis
- [VirusTotal – File Scanner](https://www.virustotal.com/gui/home/upload) ✅ *Used in this case* – confirmed phishing
- [AnyRun (interactive sandbox)](https://any.run/)
- [Joe Sandbox](https://www.joesandbox.com/)

### 🧰 All-in-One Platform
- [Hybrid Analysis](https://www.hybrid-analysis.com/) – deep malware, behavior, and threat intelligence

### 🧪 Offline Static Analysis (Optional)
- `oletools` → Analyze macros in `.docx`:
  ```bash
  pip install oletools
  olevba CanIPhish-Word-Attachment.docx
