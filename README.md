# 🔎 Digital Forensics Toolkit & Investigation Repository

<div align="center">

# 🛡️ DIGITAL FORENSICS

### A Practical Repository for Digital Investigation, Evidence Analysis & Cyber Forensics

**Created & Maintained by [SALMAAN](https://github.com/salmaanfarisshaik-art)**

[![GitHub](https://img.shields.io/badge/GitHub-SALMAAN-181717?style=for-the-badge&logo=github)](https://github.com/salmaanfarisshaik-art)
[![Domain](https://img.shields.io/badge/Domain-Digital%20Forensics-0A66C2?style=for-the-badge&logo=hackthebox&logoColor=white)](https://github.com/salmaanfarisshaik-art/Digital-Forensics)
[![Cybersecurity](https://img.shields.io/badge/Focus-Cybersecurity-00C853?style=for-the-badge&logo=protonvpn&logoColor=white)](https://github.com/salmaanfarisshaik-art/Digital-Forensics)
[![Repository](https://img.shields.io/badge/Repository-Public-2EA44F?style=for-the-badge&logo=github)](https://github.com/salmaanfarisshaik-art/Digital-Forensics)

</div>

---

## 📌 About This Repository

**Digital Forensics** is a practical cybersecurity repository created by **SALMAAN** to organize tools and resources used throughout a digital forensic investigation lifecycle.

Digital forensics is the disciplined process of **identifying, acquiring, preserving, examining, analyzing, documenting, and presenting digital evidence**. It can involve computers, storage devices, mobile devices, networks, files, memory, applications, and other digital artifacts.

This repository brings together a collection of commonly used forensic and security tools, providing a structured starting point for learning and performing investigations.

> **Mission:** Learn how digital evidence can be acquired, preserved, examined, analyzed, and documented using established forensic tools and workflows.

---

## 🎯 Objectives

The main objectives of this repository are:

- 🔍 Understand the fundamentals of digital forensic investigations
- 💾 Explore forensic acquisition and disk imaging
- 🧩 Analyze file systems and digital artifacts
- 🗂️ Recover and examine deleted or lost data
- 🧠 Understand system processes and executable behavior
- 🌐 Analyze network traffic and communications
- 📧 Examine email and mail-header information
- 📱 Explore mobile-device forensic acquisition concepts
- 🕵️ Analyze suspicious files and binaries
- 🖼️ Understand steganography and hidden-data detection
- 🛠️ Build familiarity with industry-used forensic tools
- 📝 Develop a structured and repeatable investigation methodology

---

# 🧭 Digital Forensics Investigation Lifecycle

A forensic investigation should follow a controlled and repeatable process.

```text
                    ┌───────────────────────┐
                    │   INCIDENT / EVENT    │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │  1. IDENTIFICATION    │
                    │ Evidence & Scope      │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │   2. ACQUISITION      │
                    │ Image / Collect Data  │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │   3. PRESERVATION     │
                    │ Integrity & Hashing   │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │     4. EXAMINATION     │
                    │ Extract Artifacts     │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │      5. ANALYSIS      │
                    │ Correlate Evidence   │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │   6. DOCUMENTATION    │
                    │ Findings & Timeline  │
                    └───────────┬───────────┘
                                │
                                ▼
                    ┌───────────────────────┐
                    │    7. PRESENTATION    │
                    │ Final Forensic Report│
                    └───────────────────────┘
```

---

# 🗂️ Repository Structure

The repository is organized into dedicated directories for different forensic and cybersecurity utilities:

```text
Digital-Forensics/
│
├── 📱 AFLogical OSE/
│   └── Android forensic acquisition / mobile evidence
│
├── 🔬 Autopsy/
│   └── Digital forensic investigation and artifact analysis
│
├── 💽 FTK Imager/
│   └── Forensic imaging and evidence acquisition
│
├── 🧠 Ghidra/
│   └── Reverse engineering and binary analysis
│
├── 📧 Mail Header Analyzer/
│   └── Email header investigation and analysis
│
├── ⚙️ Process-Explorer/
│   └── Windows process and system activity investigation
│
├── 🧩 SluethKit/
│   └── File-system forensic analysis
│
├── 🖼️ Steganography/
│   └── Hidden-data and steganographic analysis
│
├── 💾 TestDisk/
│   └── Partition and data recovery utilities
│
└── 🌐 Wire Shark/
    └── Network traffic and packet analysis
```

> **Note:** `SluethKit` and `Wire Shark` are retained above using the directory names currently present in the repository. The standard tool names are **The Sleuth Kit** and **Wireshark**.

---

# 🛠️ Tools & Technologies

## 1. 📱 AFLogical OSE

**AFLogical OSE (Open Source Edition)** is associated with Android forensic acquisition.

It can be used to extract supported Android artifacts such as:

- Call logs
- Contacts
- SMS
- MMS
- Related mobile-device data

### Forensic Area

`Mobile Device Forensics`

### Typical Investigation Flow

```text
Android Device
      │
      ▼
AFLogical OSE
      │
      ▼
Evidence Extraction
      │
      ▼
Collected Artifacts
      │
      ▼
Forensic Examination
```

AFLogical OSE is particularly useful for understanding the mobile-forensics acquisition stage.

---

# 2. 🔬 Autopsy

**Autopsy** is a digital forensics platform and graphical interface built around The Sleuth Kit and other forensic components.

It can be used for structured examination of forensic data sources.

### Common Uses

- Disk-image analysis
- File-system examination
- Deleted-file recovery
- Keyword searching
- Timeline analysis
- Hash-based examination
- Web and user-artifact analysis
- Registry and operating-system artifact examination
- Case management
- Report generation

### Typical Workflow

```text
Forensic Image
      │
      ▼
Create Case
      │
      ▼
Add Data Source
      │
      ▼
Run Ingest Modules
      │
      ▼
Artifact Extraction
      │
      ▼
Analysis & Correlation
      │
      ▼
Findings / Report
```

Autopsy is useful for bringing multiple forensic examination activities together inside a case-based investigation environment.

---

# 3. 💽 FTK Imager

**FTK Imager** is commonly used for forensic evidence acquisition, imaging, previewing, and verification.

### Common Uses

- Creating forensic disk images
- Previewing storage media
- Acquiring selected evidence
- Working with forensic image formats
- Verifying evidence integrity
- Examining files and folders without directly modifying the original evidence

### Basic Acquisition Concept

```text
Original Evidence
       │
       ▼
Forensic Acquisition
       │
       ▼
Forensic Image
       │
       ├── Hash Verification
       │
       └── Examination Copy
```

The core principle is to preserve the original evidence and perform analysis on an appropriate forensic copy.

---

# 4. 🧠 Ghidra

**Ghidra** is a software reverse-engineering framework that can assist with the analysis of executable programs and binaries.

### Common Uses

- Static binary analysis
- Disassembly
- Decompilation
- Function identification
- String analysis
- Control-flow examination
- Suspicious executable investigation
- Malware-analysis support

### Forensic Workflow

```text
Suspicious Binary
       │
       ▼
Hash / Identification
       │
       ▼
Ghidra Analysis
       │
       ├── Strings
       ├── Functions
       ├── Imports
       ├── Decompiled Code
       └── Control Flow
       │
       ▼
Behavioral / Technical Findings
```

Ghidra is especially valuable when a forensic investigation identifies an executable that requires deeper technical examination.

---

# 5. 📧 Mail Header Analyzer

Email headers contain technical information that can help investigators understand how an email travelled through mail infrastructure.

### Investigation Areas

- Sender information
- Recipient information
- Message identifiers
- Mail servers
- Routing information
- Received headers
- Timestamps
- Authentication-related fields
- Potential indicators of suspicious email activity

### Basic Analysis Flow

```text
Email
 │
 ▼
Extract Headers
 │
 ▼
Analyze Routing Information
 │
 ▼
Review Timestamps
 │
 ▼
Inspect Authentication Fields
 │
 ▼
Correlate with Other Evidence
```

> Header analysis should be treated as one evidence source and interpreted together with other forensic artifacts.

---

# 6. ⚙️ Process Explorer

**Process Explorer** is a Windows system utility useful for examining running processes and their relationships.

### Investigation Areas

- Running processes
- Parent-child process relationships
- Process properties
- Loaded components
- System activity
- Suspicious process behavior
- Process identification

### Process Investigation Concept

```text
System Activity
      │
      ▼
Running Processes
      │
      ▼
Parent / Child Relationships
      │
      ▼
Process Details
      │
      ▼
Suspicious Activity Identification
```

This can support live-system triage and help an investigator understand process activity before deeper forensic analysis.

---

# 7. 🧩 The Sleuth Kit

The repository contains a directory named `SluethKit`; the standard project name is **The Sleuth Kit (TSK)**.

The Sleuth Kit is a collection of command-line tools and libraries for forensic analysis of disk images and file systems.

### Common Forensic Areas

- File-system analysis
- Partition analysis
- File metadata
- Deleted-file investigation
- Directory structures
- Disk-image examination
- Timeline-related analysis

### Relationship with Autopsy

```text
              ┌───────────────┐
              │  AUTOPSY      │
              │ GUI / Case    │
              └───────┬───────┘
                      │
                      ▼
              ┌───────────────┐
              │ SLEUTH KIT    │
              │ Forensic      │
              │ Components    │
              └───────┬───────┘
                      │
                      ▼
              Disk / File System
                    Analysis
```

The Sleuth Kit provides important underlying forensic functionality used in many examination workflows.

---

# 8. 🖼️ Steganography

The **Steganography** section focuses on the concept of hiding information inside another digital medium.

Possible carrier media include:

- Images
- Audio
- Video
- Documents
- Other digital files

### Investigation Concept

```text
Carrier File
     │
     ▼
Steganographic Examination
     │
     ├── File Properties
     ├── Metadata
     ├── Statistical Analysis
     └── Hidden-Data Indicators
     │
     ▼
Potential Embedded Information
```

Steganography analysis can be useful when investigators suspect that information has been concealed inside apparently normal files.

---

# 9. 💾 TestDisk

**TestDisk** is a data-recovery utility commonly used to work with lost partitions and recover data in appropriate situations.

### Common Uses

- Lost-partition recovery
- Partition-table examination
- File-system recovery support
- Recovery from damaged or inaccessible partitions

### Recovery Concept

```text
Storage Media
      │
      ▼
Partition / File-System Examination
      │
      ▼
Identify Recoverable Structures
      │
      ▼
Recovery Operation
      │
      ▼
Recovered Data
```

For forensic work, recovery actions should be performed carefully and documented so that evidence handling remains controlled.

---

# 10. 🌐 Wireshark

The repository contains a directory named `Wire Shark`; the standard tool name is **Wireshark**.

Wireshark is a network protocol analyzer used to capture and examine network traffic.

### Common Uses

- Packet capture analysis
- Protocol inspection
- IP communication analysis
- TCP/UDP investigation
- DNS analysis
- HTTP/HTTPS-related investigation
- Suspicious connection analysis
- Network troubleshooting
- Incident-response support

### Network Forensics Flow

```text
Network Traffic
      │
      ▼
Packet Capture
      │
      ▼
Wireshark
      │
      ▼
Protocol Analysis
      │
      ▼
Conversation / Endpoint Analysis
      │
      ▼
Indicators & Findings
```

Network evidence can be correlated with host, file, email, and process artifacts to reconstruct an incident more accurately.

---

# 🔗 How the Tools Work Together

The tools in this repository can support different stages of an investigation rather than operating as isolated utilities.

```text
                     DIGITAL FORENSICS
                            │
          ┌─────────────────┼─────────────────┐
          │                 │                 │
          ▼                 ▼                 ▼
       HOST / DISK       NETWORK           MOBILE
          │                 │                 │
          ▼                 ▼                 ▼
    FTK Imager          Wireshark       AFLogical OSE
          │
          ▼
       Autopsy
          │
          ▼
     Sleuth Kit
          │
          ├──────────────┐
          │              │
          ▼              ▼
     TestDisk         Evidence
                      Recovery
          │
          ▼
   Suspicious Files
          │
          ▼
       Ghidra
          │
          ▼
 Reverse Engineering
```

Additional supporting analysis can include:

- **Mail Header Analyzer** → email investigations
- **Process Explorer** → live process investigation
- **Steganography** → hidden-data examination

---

# 🧪 Suggested Investigation Workflow

A complete investigation can be structured as follows:

### Phase 1 — Preparation

- Define the investigation scope
- Identify the evidence source
- Record case information
- Prepare a controlled analysis environment

### Phase 2 — Identification

Identify potentially relevant:

- Devices
- Disk images
- Files
- Network captures
- Emails
- Mobile artifacts
- Executables
- System processes

### Phase 3 — Acquisition

Acquire evidence using appropriate forensic procedures.

Examples:

- FTK Imager → disk acquisition
- AFLogical OSE → supported Android artifact acquisition
- Wireshark → network capture

### Phase 4 — Preservation

Protect evidence integrity through:

- Hashing
- Write protection where appropriate
- Evidence copies
- Documentation
- Chain-of-custody records

### Phase 5 — Examination

Extract and organize relevant artifacts using:

- Autopsy
- The Sleuth Kit
- TestDisk
- Wireshark
- Mail Header Analyzer
- Other appropriate tools

### Phase 6 — Analysis

Correlate evidence across different sources.

For example:

```text
File Timestamp
      +
Process Activity
      +
Network Connection
      +
Email Evidence
      +
Recovered File
      ↓
Incident Timeline
```

### Phase 7 — Specialized Analysis

If necessary:

- Ghidra → binary/reverse engineering
- Steganography tools → hidden-data examination
- Process Explorer → process investigation

### Phase 8 — Documentation

Record:

- Evidence examined
- Tools used
- Procedures followed
- Relevant observations
- Hash values
- Timeline information
- Screenshots
- Findings
- Limitations

### Phase 9 — Reporting

Prepare a clear forensic report containing:

1. Case information
2. Scope
3. Evidence sources
4. Acquisition methodology
5. Examination methodology
6. Findings
7. Timeline
8. Indicators
9. Supporting screenshots
10. Conclusion
11. References

---

# 📊 Forensic Evidence Categories

| Evidence Category | Examples | Repository Tools |
|---|---|---|
| 💽 Disk Evidence | Disk images, partitions, file systems | FTK Imager, Autopsy, Sleuth Kit |
| 📁 File Evidence | Files, deleted files, metadata | Autopsy, Sleuth Kit, TestDisk |
| 🌐 Network Evidence | Packets, connections, protocols | Wireshark |
| 📧 Email Evidence | Headers, routing information | Mail Header Analyzer |
| 📱 Mobile Evidence | Calls, contacts, messages | AFLogical OSE |
| ⚙️ Process Evidence | Running processes, process relationships | Process Explorer |
| 🧠 Binary Evidence | Executables, suspicious binaries | Ghidra |
| 🖼️ Hidden Evidence | Embedded / concealed information | Steganography tools |

---

# 🔐 Evidence Integrity

Digital evidence must be handled carefully because unintended changes can affect its reliability.

Important practices include:

### 1. Preserve the Original

Do not perform unnecessary modifications to the original evidence source.

### 2. Use Forensic Copies

Whenever possible, perform examination on an appropriate forensic copy.

### 3. Verify Integrity

Cryptographic hashes can be used to verify whether data has changed.

Commonly encountered hashing algorithms include:

```text
MD5
SHA-1
SHA-256
```

Modern investigations should generally prefer stronger algorithms such as SHA-256 where appropriate.

### 4. Maintain Documentation

Every important forensic action should be recorded.

### 5. Maintain Chain of Custody

Record:

```text
Who
  ↓
Collected
  ↓
What
  ↓
When
  ↓
Where
  ↓
How
  ↓
Where Stored
  ↓
Who Accessed
```

---

# 🧰 Recommended Analysis Environment

A dedicated forensic analysis environment is recommended.

### Operating Systems

- Windows
- Linux
- Specialized forensic distributions where appropriate

### Useful Supporting Software

- VirtualBox / VMware
- Git
- Python
- PowerShell
- Command Prompt / Terminal
- Hashing utilities
- PDF/report-generation utilities

### Isolation

When examining potentially malicious or suspicious files:

```text
Host System
     │
     ▼
Isolated / Controlled Environment
     │
     ▼
Forensic Examination
     │
     ▼
Evidence Collection
```

Never execute unknown malware on a production or personal system.

---

# 📚 Learning Areas Covered

This repository can be used as a practical learning reference for:

- Digital forensics fundamentals
- Computer forensics
- Disk forensics
- File-system forensics
- Mobile forensics
- Network forensics
- Email forensics
- Malware / binary analysis
- Reverse engineering
- Data recovery
- Steganography
- Incident-response support
- Evidence preservation
- Forensic documentation

---

# 🎓 Learning Outcomes

After working through the tools and concepts in this repository, a learner should be able to understand:

- How digital evidence is collected
- Why evidence integrity matters
- How forensic disk images are created and examined
- How file systems can be analyzed
- How deleted information may be investigated
- How network packets can be examined
- How email headers provide investigative clues
- How processes can be inspected on Windows
- How suspicious binaries can be reverse engineered
- How hidden information can be investigated
- How forensic findings can be documented

---

# ⚖️ Legal & Ethical Use

This repository is intended for:

- 🎓 Education
- 🧪 Authorized laboratory experiments
- 🔐 Cybersecurity research
- 🕵️ Digital forensic training
- 🛡️ Incident-response learning
- 💻 Analysis of systems and evidence for which you have permission

### Important

Do **not** use these tools to access, monitor, modify, recover, or analyze data belonging to another person or organization without proper authorization.

Digital forensic tools are powerful. Their use should comply with applicable laws, organizational policies, evidence-handling procedures, and ethical standards.

---

# 🚀 Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/salmaanfarisshaik-art/Digital-Forensics.git
```

## 2. Enter the Repository

```bash
cd Digital-Forensics
```

## 3. Explore the Tool Categories

```text
AFLogical OSE/
Autopsy/
FTK Imager/
Ghidra/
Mail Header Analyzer/
Process-Explorer/
SluethKit/
Steganography/
TestDisk/
Wire Shark/
```

## 4. Choose the Investigation Area

For example:

```text
Disk Investigation      → FTK Imager + Autopsy + Sleuth Kit
Network Investigation   → Wireshark
Mobile Investigation    → AFLogical OSE
Binary Investigation    → Ghidra
Process Investigation   → Process Explorer
Email Investigation     → Mail Header Analyzer
Recovery Investigation  → TestDisk
Hidden Data Investigation → Steganography
```

---

# 🗺️ Future Improvements

The repository can be expanded with additional material such as:

- [ ] Step-by-step forensic lab manuals
- [ ] Practical case studies
- [ ] Sample forensic images
- [ ] Network PCAP exercises
- [ ] Mobile-forensics exercises
- [ ] Windows forensic artifacts
- [ ] Linux forensic artifacts
- [ ] Memory-forensics workflows
- [ ] Malware-analysis labs
- [ ] Automated forensic scripts
- [ ] Evidence-hashing utilities
- [ ] Timeline-analysis examples
- [ ] IOC extraction workflows
- [ ] Forensic report templates
- [ ] Screenshots and investigation walkthroughs
- [ ] DFIR playbooks
- [ ] Case-study documentation

---

# 📁 Suggested Future Repository Structure

As the repository grows, a scalable structure could look like:

```text
Digital-Forensics/
│
├── README.md
│
├── 01-Mobile-Forensics/
│   └── AFLogical-OSE/
│
├── 02-Disk-Forensics/
│   ├── FTK-Imager/
│   ├── Autopsy/
│   ├── Sleuth-Kit/
│   └── TestDisk/
│
├── 03-Network-Forensics/
│   └── Wireshark/
│
├── 04-Email-Forensics/
│   └── Mail-Header-Analyzer/
│
├── 05-Process-Forensics/
│   └── Process-Explorer/
│
├── 06-Reverse-Engineering/
│   └── Ghidra/
│
├── 07-Steganography/
│
├── 08-Labs/
│
├── 09-Case-Studies/
│
├── 10-Reports/
│
└── 11-References/
```

This structure is a suggested organization for future expansion; the current repository structure is described above based on the directories currently visible in the GitHub repository.

---

# 📖 References & Further Reading

The following resources are useful for learning digital forensics and the tools represented in this repository:

- **NIST Computer Security Resource Center (CSRC)** — Digital forensics and incident-response guidance
- **The Sleuth Kit** — Open-source forensic analysis framework
- **Autopsy** — Digital forensics platform
- **Ghidra** — Software reverse-engineering framework
- **Wireshark** — Network protocol analyzer
- **TestDisk** — Data recovery and partition recovery utility
- **AFLogical OSE** — Open-source Android forensic acquisition project

For tool-specific installation instructions and current documentation, always consult the respective official project documentation.

---

# 👨‍💻 Author

<div align="center">

## **SALMAAN**

### Digital Forensics | Cybersecurity | Security Research

**Repository:**  
https://github.com/salmaanfarisshaik-art/Digital-Forensics

**GitHub Profile:**  
https://github.com/salmaanfarisshaik-art

</div>

---

# ⭐ Support the Project

If this repository helps you learn digital forensics:

- ⭐ Star the repository
- 🍴 Fork it for your own learning
- 🐛 Report issues
- 💡 Suggest improvements
- 📚 Add useful forensic resources
- 🔬 Share educational case studies

---

<div align="center">

### 🔎 Investigate. Preserve. Analyze. Document.

**Built for learning Digital Forensics — by SALMAAN.**

---

`Digital Evidence → Acquisition → Preservation → Examination → Analysis → Documentation → Presentation`

</div>
