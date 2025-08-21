**Digital Forensics Terminology** 
---


### **Acquisition**

The process of creating an exact, bit-by-bit copy (or image) of digital media (e.g., hard drive, USB) to preserve the original evidence. This copy is then used for forensic examination while maintaining the integrity of the source.

---

### **eDiscovery**

Short for **electronic discovery**. It refers to the process of identifying, collecting, and producing electronically stored information (ESI) in response to a legal request or investigation.

---

### **Exhibit**

Any digital media or device (e.g., computer, phone, USB drive) seized during an investigation is referred to as an **exhibit**. Each exhibit is typically cataloged, labeled, and tracked to maintain the chain of custody.

---

### **Hashing**

A technique used to verify data integrity. It uses cryptographic algorithms such as **MD5**, **SHA-1**, or **CRC** to generate a unique value (hash) for a data set. If two data sets produce the same hash, they are considered identical.

---

### **Image**

In digital forensics, an **image** refers to a complete, bit-level copy of a digital storage device. This includes all files, folders, partitions, and unallocated space. It is often used in place of the original media during analysis to protect the evidence.

---

### **Live Analysis**

A method of forensic examination performed on a system that is powered on and possibly running. This allows access to volatile data such as RAM, active network connections, and running processes, which are lost when the system is shut down.

---

### **Unallocated Space**

The portion of a storage device not currently assigned to any active file. Although not in use, it may still contain remnants of deleted files or data fragments and is often analyzed for hidden or deleted information.

---

### **Chain of Custody**

A documented process that tracks the handling of digital evidence from the moment it is collected until it is presented in court. It ensures the integrity and admissibility of the evidence by recording who handled it, when, and how.

---

### **Metadata**

Data about data. In digital forensics, metadata refers to information such as file creation dates, modification times, user access logs, and authorship details. It can provide insight into file activity and timelines.

---

### **Volatile Data**

Information that is stored in temporary memory (like RAM) and lost when a system is powered down. It includes active processes, open files, clipboard contents, and network connections. Volatile data must be collected during live analysis.

---

### **Write Blocker**

A forensic tool used during acquisition to prevent any data from being written to the source media. It ensures that the original evidence remains unchanged while being copied or analyzed.

---

### **Timeline Analysis**

A method of reconstructing user or system activity by organizing file system and log data (like metadata timestamps) chronologically. It helps investigators understand the sequence of events on a system.

---

### **Data Carving**

A technique used to recover files from unallocated space or damaged media without relying on the file system structure. It identifies and extracts data based on known file signatures.

---

### **Forensic Image Verification**

The process of confirming that a forensic image (copy) matches the original media, typically using hash values. Matching hash values prove that no data has been altered.

---

### **Slack Space**

The unused space in a disk cluster between the end of a file and the end of the cluster. It may contain leftover data from previously deleted files and can be analyzed for hidden information.

---

### **Steganography**

A method of concealing data within other seemingly innocuous files, such as hiding text in an image or audio file. Detecting steganography is part of advanced forensic analysis.

---


