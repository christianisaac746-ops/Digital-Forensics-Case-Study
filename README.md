**Digital Forensics Case Study:** ABC Tech Confidential Data Breach
**Course:** Digital Forensics in Cybersecurity - D829 Date: November 19, 2025 Analyst: Christian Rooks

**I. Introduction and Case Summary**
This document provides a formal and thorough account of a confidential data breach incident at ABC Tech. The primary concern was unauthorized access to, and the potential falsification or exfiltration of, crucial files from a suspected Windows 11 workstation.

A. Investigation Scope and Objectives
The investigation was a formal, host-based forensic analysis limited exclusively to the suspected Windows 11 workstation.

The primary objectives were to:

Extract deleted files and documents from user directories.

Analyze system event logs to identify suspicious activity.

Recover browser activity artifacts, including cookies and cached files.

Generate a forensic report detailing the findings.

B. Tools and Methodology
The investigation adhered strictly to the industry-standard forensic process (Preparation, Collection, Examination, Analysis, and Reporting).

<img width="686" height="356" alt="Image" src="https://github.com/user-attachments/assets/91de5292-a3e3-4b9b-94d4-05b15e01f97a" />

**II. Legal and Regulatory Framework**
The investigation was governed by a comprehensive framework of local laws, industry standards, and company policies to ensure the evidence gathering process was lawful, ethical, and forensically sound.

A. Applicable Laws and Regulations
The investigation is mandated to comply with several categories of legislation, depending on the nature of the compromised data:


Data Protection Regulations: General Data Protection Regulation (GDPR) or California Consumer Privacy Act (CCPA) if Personally Identifiable Information (PII) is involved.




Sector-Specific Laws: Health Insurance Portability and Accountability Act (HIPAA) for Protected Health Information (PHI) or Gramm-Leach-Bliley Act (GLBA) for financial consumer data.



Financial Reporting: Sarbanes-Oxley Act (SOX) if ABC Tech is a publicly listed corporation, to maintain the trustworthiness of financial data.


B. Industry Standards
The analysis aligned with global industry standards for technical soundness and defensibility:


NIST Special Publication (SP) 800-86: Provides recommendations for integrating forensic analysis into overall organizational incident response.



ISO/IEC 27043:2015: Outlines principles and procedures for investigating incidents and handling evidence to maintain consistency and legal correctness.


C. Organizational Policies
Internal company documentation provided the legal authority and guidelines:


Incident Response Plan (IRP): Formal authorization for the probe and details for the stages of containment, eradication, and recovery.


Acceptable Use Policy (AUP): Provided the legal basis for searching the employee's company-owned workstation, which is subject to monitoring.


Data Retention and Handling Policies: Guided the classification of compromised data and established the mandatory secure methodology for retaining the evidence.

**III. Evidence Collection and Artifact Recovery**
The forensic image (wgu_scenario.001) was loaded into Autopsy and FTK Imager. All analysis was conducted on the forensic working copies (least disturbance principle).

The following critical digital artifacts were successfully extracted to the Desktop:

<img width="494" height="691" alt="Image" src="https://github.com/user-attachments/assets/ab7b6c0d-f698-45b9-89a7-c839ed7fb008" />

**IV. Findings and Policy Violations**
The evidence points to several incidents of unauthorized activity, data exfiltration, and clear policy violations.



A. Key Findings

Explicit Intent to Exfiltrate: The recovered deleted file, secret.txt, contained the explicit instruction: "email: hacker123@gmail.com Remember to send confidential information and data to the designated email. Delete any evidence afterwards and make sure to not get caught doing me".

This is strong evidence of an intent to disseminate confidential data and actively cover up the breach.



Unauthorized Tool Use: The successful extraction of the executable file, logger.exe, from the Downloads folder indicates the presence and potential use of an unauthorized monitoring or logging tool on the corporate workstation.



Data Compromise: The recovery of other potentially sensitive corporate files, such as balance_sheet.xlsx and todo.docx, from the Downloads and Documents folders, respectively, indicates unauthorized access to or manipulation of proprietary information.

B. Policy Violations Summary

<img width="688" height="333" alt="Image" src="https://github.com/user-attachments/assets/2bcf9488-2399-4dd8-990e-7ab997ccb8fe" />

**V. Conclusion**
The forensic investigation has successfully achieved its objectives by recovering numerous digital artifacts that clearly demonstrate unauthorized activity on the Windows 11 workstation. The most compelling evidence is the recovery of the deleted file secret.txt, which provides a written confession of intent to exfiltrate confidential data and actively cover up the crime.

The combined evidence from deleted files, unauthorized executables, and browser artifacts strongly supports the conclusion that ABC Tech's policies have been severely violated, and the breach of confidential information is highly probable.

**Disclaimer & Terms of Use**

  + Educational Purposes Only: The content of this laboratory walkthrough is intended solely for educational and portfolio demonstration purposes.

  + Ethical Standards: All forensic techniques were performed in a controlled, virtualized environment. These methods should only be applied to systems where you have explicit, written legal authorization. Unauthorized access to computer systems is illegal and unethical.

  + No Liability: The author assumes no responsibility for any actions taken by individuals based on the information provided in this document. Use of these techniques is at your own risk.







