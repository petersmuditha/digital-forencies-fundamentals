# **Digital Forensics: From Crime Scene to Courtroom**

## **Introduction to Digital Forensics**

Forensics is the application of methods and procedures to investigate and solve crimes. The branch of forensics that investigates cyber crimes is known as **digital forensics**. Cyber crime is any criminal activity conducted on or using a digital device. Several tools and techniques are used to investigate digital devices thoroughly after any crime to find and analyze evidence for necessary legal action.

Digital devices have solved many of our problems. Communication all around the globe is just a matter of a text or call. Due to the vast usage of digital devices, besides making life easier, an increase in digital crimes—cyber crimes—has also been observed. A variety of crimes are committed using digital devices.

---

## **Real-World Case Example**

![image alt](https://github.com/petersmuditha/digital-forencies-fundamentals/blob/acece3ddb4dc331b5c032d0ec3b8e74032e43a22/Cattura%2099.PNG)🏦
![image alt](https://github.com/petersmuditha/digital-forencies-fundamentals/blob/43b2915a5b0480bae6e73e4235fa077e82ce89d2/Cattura100.PNG)
Case Background
Law enforcement agencies raided a bank robber's residence with proper search warrants. Multiple digital devices were seized, including:

Laptop

Mobile phone

External hard drive

USB flash drive

The digital forensics team received these devices for analysis in their secure forensic lab.

Step 1: Initial Evidence Assessment
Command Used: ls - List Directory Contents
bash
Command Explanation:

Path: /evidence/bank-robbery-case/ - Evidence storage directory

Purpose: Initial inventory of seized digital evidence

Step 2: PDF Document Analysis
Command Used: pdfinfo - PDF Metadata Extraction
bash
root@forensics-lab:~# pdfinfo ransom-letter.pdf
Command Explanation:

pdfinfo: Tool from Poppler utilities suite for PDF analysis

File: ransom-letter.pdf - Suspect's ransom note

Purpose: Extract metadata and document properties

Step 3: Image Metadata Analysis
Command Used: exiftool - Comprehensive Metadata Extraction
Command Explanation:

exiftool: Perl-based tool for reading/writing metadata

File: letter-image.jpg - Potential evidence image

Purpose: Extract EXIF, IPTC, XMP, and other metadata



---

## **The Digital Forensics Process (NIST Framework)**

The National Institute of Standards and Technology (NIST) defines a general process for every case. The NIST works on defining frameworks for different areas of technology, including cyber security, where they introduce the process of digital forensics in **four phases**:

### **1. Collection**
The first phase of digital forensics is data collection. Identifying all the devices from which the data can be collected is essential. Usually, an investigator can find personal computers, laptops, digital cameras, USBs, etc., on the crime scene. It is also necessary to ensure the original data is not tampered with while collecting the evidence and to maintain a proper document containing the collected items' details.

### **2. Examination**
The collected data may overwhelm investigators due to its size. This data usually needs to be filtered, and the data of interest needs to be extracted. For example, as an investigator, you collected all the media files from a digital camera on the crime scene. You may only require some of the media as you are concerned with the media recorded on a specific date and time.

### **3. Analysis**
This is a critical phase. The investigators now have to analyze the data by correlating it with multiple pieces of evidence to draw conclusions. The analysis depends upon the case scenario and available data. The analysis aims to extract the activities relevant to the case chronologically.

### **4. Reporting**
In the last phase of digital forensics, a detailed report is prepared. This report contains the investigation's methodology and detailed findings from the collected evidence. It may also contain recommendations. This report is presented to law enforcement and executive management.

---

## **Fields of Digital Forensics**


As part of the collection phase, we saw that various pieces of evidence can be found at the crime scene. Analyzing these multiple categories of evidence requires various tools and techniques. There are different types of digital forensics, all with their own collection and analysis methodologies. Some of the most common types are listed below.

| **Field** | **Description** |
|-----------|-----------------|
| **Computer Forensics** | Investigating computers and storage devices |
| **Mobile Forensics** | Extracting evidence from mobile devices |
| **Network Forensics** | Analyzing network traffic and logs |
| **Database Forensics** | Investigating database intrusions |
| **Cloud Forensics** | Examining cloud-based evidence |
| **Email Forensics** | Analyzing emails for fraud |

---

## **Evidence Acquisition Best Practices**

### **Proper Authorization**
The forensics team should obtain authorization from the relevant authorities before collecting any data.

### **Chain of Custody**
A formal document that tracks evidence handling from collection to court.

### **Use of Write Blockers**
Prevents alteration of original evidence during acquisition.

---
## **Integration with SOC Processes**

### **Key SOC Processes**
1. **Alert Triage** 🔴
2. **Incident Response** 🛡️
3. **Forensics** 🔎

### **Essential SOC Technologies**

| **Category** | **Tools** |
|--------------|-----------|
| **Visibility** | SIEM, Log Management |
| **Endpoint Security** | EDR, EPP, AV |
| **Network Security** | Firewalls, IDS/IPS |
| **Automation** | SOAR, XDR |
| **Threat Intel** | TI Platforms |

### **Key Performance Indicators (KPIs)**
- **MTTD**: Mean Time to Detect
- **MTTR**: Mean Time to Respond
- **MTTI**: Mean Time to Investigate

  Case Conclusion:

This digital forensics investigation successfully identified Ann Gree Shepherd as the primary suspect through PDF metadata analysis and uncovered evidence of image manipulation via timestamp inconsistencies in the photograph. The tools pdfinfo and exiftool provided critical technical evidence linking the suspect to the crime, while maintaining proper forensic protocols. The case demonstrates how digital evidence—when collected and analyzed correctly—can be decisive in criminal investigations.





