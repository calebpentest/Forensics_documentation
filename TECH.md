# **Windows Forensic Investigation Workflow**

---

## **1. Preparation**

* **Define scope & objectives**
  What are you trying to prove, detect, or uncover?

*  **Obtain proper authorization**
  Ensure you have legal authority (e.g., warrant, internal policy, consent).

* **Prepare tools and environment**

  * Forensic workstation (isolated & secured)
  * Write blockers
  * Forensic software (FTK, Autopsy, etc.)

---

## **2. Acquisition**

*  **Secure the scene**
  Prevent tampering or remote access (e.g., disconnect from network).

*  **Decide: live vs. dead acquisition**

  * *Live:* RAM, active sessions, volatile data (if system is on)
  * *Dead:* Disk image (if system is powered off or you shut it down safely)

*  **Create forensic images**

  * Use tools like FTK Imager, dd, or Guymager
  * Use **write blockers**
  * Record hash values (MD5, SHA-1) before and after imaging

---

## **3. Verification**

* **Hash verification**
  Ensure the image matches the original (bit-for-bit identical)

* **Chain of custody**
  Log each handoff, access, or interaction with evidence

---

## **4. Analysis**

This is the core phase. Analyze artifacts relevant to the case:

*  **User activity**

  * Browser history
  * Recent documents
  * USB device history
  * Logon/logoff times

*  **System artifacts**

  * Event logs
  * Prefetch files
  * Installed programs and services
  * Registry analysis (NTUSER.DAT, SYSTEM)

*  **Deleted file recovery**

  * Unallocated space
  * Slack space
  * Recycle Bin

*  **Correlate timelines**

  * File system timestamps (MFT)
  * Event logs
  * Prefetch execution times

* **Memory analysis (if applicable)**

  * RAM dump
  * Passwords, processes, network connections

---

## **5. Reporting**

* Create a **clear, factual report**

  * Objective findings only
  * Screenshots of artifacts
  * Hash values
  * Tools used and methodology

* **Conclusions** (only if requested)

  * Based on evidence, not assumptions

*  **Attach appendices**

  * Hash values, timelines, logs, screenshots, etc.

---

#  **Case Documentation Format (Sample Outline)**

Here’s a professional structure you can use or adapt:

---

### **1. Case Overview**

* Case Number:
* Investigator(s):
* Date Opened:
* Summary of Incident:

---

### **2. Scope and Objectives**

* What is being investigated?
* What are the goals?

---

### **3. Evidence Summary**

* Exhibit ID:
* Description: (e.g., Dell laptop, Serial: XXXXXX)
* Acquisition Date & Time:
* Hashes (MD5/SHA-1):
* Tool(s) Used for Imaging:

---

### **4. Forensic Methodology**

* Acquisition Method: (live or dead)
* Tools Used:
* Steps Taken:

---

### **5. Analysis & Findings**

Organize this by artifact type or timeline:

#### a. Timeline of Events

#### b. User Activity

#### c. System Artifacts

#### d. Suspicious Files or Programs

#### e. Recovered or Deleted Files

#### f. Registry or Configuration Changes

---

### **6. Conclusion**

* Summarize findings
* Be factual and concise
* Avoid speculation unless directed

---

### **7. Appendices**

* Full hash list
* Screenshots
* Log files
* Tool output
* Chain of custody log

---


