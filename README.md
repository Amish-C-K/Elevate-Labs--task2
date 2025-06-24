# 📧 Phishing Email Analysis – Fake ZipRecruiter Job Offer

This project contains a full analysis of a **simulated phishing email** designed to mimic a job offer from ZipRecruiter. The email was analyzed as part of a cybersecurity training task to identify social engineering tactics and phishing indicators.

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

## 🔍 Phishing Indicators

| # | Indicator | Details |
|--|-----------|---------|
| 1 | 🕵️ Spoofed Domain | Sender uses `authwebmail.com`, not an official `ziprecruiter.com` domain. |
| 2 | 🎯 Too-Good-To-Be-True Offer | Claims an unsolicited high-paying role ($275k–$325k) with vague justification. |
| 3 | 📎 Suspicious Attachment | `.docx` file prompts user to "Enable Editing" — a common macro malware trick. |
| 4 | ⚠️ Urgency | Pushes for immediate response (“intro call this week”) to pressure the recipient. |
| 5 | 🧷 Broken Content | Word document contains missing images — often seen in phishing lures. |
| 6 | 🔗 No Verifiable Links | No URLs pointing to real ZipRecruiter or PaySphere domains; no way to verify the offer. |
| 7 | 💬 Generic Language | Mentions “LinkedIn profile” without personalization; looks automated. |

---

## 📎 Attachment Analysis

**File**: `CanIPhish-Word-Attachment.docx`

**Behavior**:
- Opens in **Microsoft Word Protected View**
- Displays: _“The linked image cannot be displayed”_
- Prompts the user to “**Enable Editing**”
- ⚠️ This technique is commonly used to **execute malicious macros** once editing is enabled

---

## 🧠 Conclusion

This email is a **classic phishing attempt**. It impersonates a well-known job platform, uses urgency and flattery to manipulate the recipient, and includes a suspicious attachment likely intended to deliver malware. Key red flags include:

- Spoofed sender domain
- Unrealistic salary claim
- Pressure for quick action
- Malicious `.docx` file with editing request

---

## 🧰 Tools Used

- Manual email inspection
- Microsoft Word (Protected View)
- Email client analysis (visual, no header data)

---

## 📷 Screenshots

This repository includes screenshots of:
- The email in the inbox
- The email content
- The opened Word document in Protected View

---

## 🛡️ Disclaimer

This project is for **educational and awareness purposes only**. It simulates a phishing scenario in a controlled environment. Do not attempt to replicate or forward phishing content in real-world settings.

---

**Author**: Ack  
**Task**: Phishing Email Analysis (Task 2)  
**Date**: June 2025
