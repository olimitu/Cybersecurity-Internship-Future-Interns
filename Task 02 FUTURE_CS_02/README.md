# 🛡️ Task 02 Phishing Email Detection & Awareness System 🔍


## 📝 Executive Summary
This project features a **technical forensic investigation** into a malicious email used in a targeted phishing campaign. Instead of relying solely on visual red flags, this analysis dives deep into **Email Header Forensics** to verify digital signatures (SPF, DKIM, DMARC) and empirically prove sender impersonation.

The goal is to move beyond "informed guessing" and provide a data-driven confirmation of a cyber threat.

---

## 🧬 Technical Stack & Frameworks

* **🛠️ Tools:** Email Header Parsers (Google Toolbox, MXToolbox), OSINT Domain Lookups.
* **📡 Protocols:** SPF (Sender Policy Framework), DKIM (DomainKeys Identified Mail), DMARC (Policy Enforcement).
* **🧠 Concepts:** Social Engineering Deconstruction, URL Obfuscation, Forensic Header Analysis.

---

## 🚩 Phishing Indicators & Business Impact

| Indicator | Technical Observation | Business Risk |
| :--- | :--- | :--- |
| **🚨 Auth Failure** | Failed **SPF, DKIM, & DMARC** checks. | **Critical:** Confirmative proof of fraud; high risk of credential harvesting or malware delivery. |
| **🎭 Identity Mismatch** | Display name `alerts@trustedbank.com` vs. Return-Path `auth-secure-mail.top`. | **High:** Exploits "Display Name Spoofing" to bypass human scrutiny and trick employees. |
| **🔓 Insecure Payload** | Link uses **unencrypted `http://`** instead of `https://`. | **High:** Data entered is transmitted in plain text, making it easily interceptable by attackers. |
| **⏳ Psychological Trigger** | Urgent claims of unauthorized withdrawals **($135.25)**. | **Medium:** Uses "Urgency Bias" to bypass rational thinking-a classic social engineering tactic. |

---

## 🧱 Defensive Guidelines (The "Human Firewall")

Building a resilient organization requires more than just software-it requires **informed users**. 💡

* **🖱️ The Hover Test:** Always hover over links to reveal the *actual* destination URL before clicking.
* **🔗 The "Direct Source" Rule:** Never use links inside an email to "verify" an account. Manually type the official address into your browser.
* **📑 Authentication Logic:** Legitimate financial institutions do not fail SPF/DMARC checks. A technical failure is a **100% confirmation** of a threat.
* **🛑 Stop, Look, Think:** If an email triggers a strong emotional response (fear or excitement), it is likely a trap.

---
### 📃 Project Evidence
* 🔗 **[Full Phishing Analysis Report]([./FUTURE_CS_02.pdf](https://github.com/olimitu/Cybersecurity-Internship-Future-Interns/blob/main/Task%2002%20FUTURE_CS_02/FUTURE_CS_02.pdf))**
