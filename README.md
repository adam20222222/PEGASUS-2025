# 🔍 Pegasus Spyware & iPhone Surveillance Tools: Educational Overview

This open-source documentation provides a **technical overview of Pegasus spyware** and other iPhone monitoring tools. It is intended for educational use by cybersecurity students, analysts, and digital rights researchers. The focus is on how high-risk surveillance implants differ from commercial mobile monitoring software.

> ⚠️ **Disclaimer:** This repository is for educational and informational purposes only. No endorsement of unauthorized access or surveillance is implied or supported.

---

## 🧨 1. Pegasus Spyware (NSO Group) – A Zero-Click Threat

**Vector Type:** Remote, zero-click exploitation via iMessage or browser components.

**Overview:**  
Pegasus is a well-documented surveillance platform developed by the NSO Group. It is known for its ability to silently infiltrate iPhones (and Androids) without requiring any user interaction. Exploits are commonly delivered via messaging services or web content, enabling full access to device data, including camera feeds, encrypted messaging, GPS, and more.

> Pegasus has been used by government clients globally and is the subject of significant human rights investigations.

**Screenshot Reference:**  
![Pegasus Sample](https://i.imgur.com/fw7x5DC.jpeg)

---

## 🕳️ 2. TriangleDB Implant – Covert Zero-Click Threat

**Vector Type:** In-memory kernel-level implant.

**Overview:**  
TriangleDB is suspected to be a memory-resident implant associated with advanced surveillance campaigns. It shares characteristics with FORCEDENTRY-style delivery mechanisms. Operating fully in-memory, it leaves no persistent disk traces, making it extremely evasive and difficult to detect in forensic analysis.

**Screenshot Reference:**  
![TriangleDB](https://pbs.twimg.com/media/GrxoHKkXMAAkVBI?format=jpg&name=large)

---

## 🛑 3. FlexiSPY – Commercial Phone Monitor (Credential-Dependent)

**Access Requirements:** Physical access or valid iCloud credentials.

**Overview:**  
FlexiSPY is a consumer-level tool marketed for parental control or employee oversight. It requires device jailbreaking or backup credential injection. Unlike Pegasus, it does not bypass iOS protections or use exploit-based access. Its usage is limited to situations where user authentication is already available.

**Screenshot Reference:**  
![FlexiSPY Dashboard](https://www.flexispy.com/common/images/screenshots/flexispy/dashboard.jpg)

---

## 🛡️ 4. mSpy – iCloud-Based Monitoring Tool

**Access Requirements:** iCloud login with backup access.

**Overview:**  
mSpy relies on iCloud data synchronization and does not exploit any iOS vulnerabilities. It functions within the limits of consent-based access and operates entirely via backup retrieval, offering monitoring of messages, contacts, and GPS with credentialed access only.

**Screenshot Reference:**  
![mSpy Dashboard](https://www.mspy.com/static/mspy/public/assets/images/redesign/features/common/big_access_picture@2x.png?v=v2)

---

## 🔐 5. EyeZy – Cloud Dashboard Monitoring

**Access Requirements:** Valid cloud account credentials.

**Overview:**  
EyeZy is designed for legitimate monitoring of synced iCloud data. It offers a dashboard-style interface for observing usage patterns, GPS data, and app activity. It does not interact directly with iOS firmware or attempt unauthorized entry. Its use is restricted to consent-based scenarios.

**Screenshot Reference:**  
![EyeZy Dashboard](https://nexspy.com/wp-content/uploads/2023/01/eyezy-dashboard.webp)

---

## ✅ Technical Comparison Summary

| Tool        | Exploit Used      | Access Needed         | Persistence | Target Audience          |
|-------------|-------------------|------------------------|-------------|---------------------------|
| Pegasus     | Zero-day, remote  | None                   | High        | State-level surveillance  |
| TriangleDB  | Kernel-level RCE  | None                   | High        | Covert cyber operations   |
| FlexiSPY    | No exploit        | Credentials + Access   | App-level   | Consumers, employers      |
| mSpy        | No exploit        | Cloud login            | App-level   | Consumers, parents        |
| EyeZy       | No exploit        | Cloud login            | Cloud-only  | Parents, guardians        |

---

## 📘 Final Notes

This project emphasizes the **technical, ethical, and legal distinctions** between:
- Government-grade spyware like **Pegasus**, which uses zero-day vulnerabilities and stealth persistence;
- Credential-based consumer monitoring apps like **FlexiSPY** or **mSpy**, which rely on prior device access.

We encourage all users to engage in **ethical research and digital rights advocacy**, and to avoid any use of this material in violation of applicable laws.

> 🛡️ This repository complies with GitHub’s Terms of Service and does not include any executable code or illegal instructions.
