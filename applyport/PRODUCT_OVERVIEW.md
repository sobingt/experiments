# 📘 Product Orientation – LinkedIn Job Applicants Exporter

**Marketing Name:** LinkedIn Job Applicants Exporter  
**Internal Codename:** ApplyPort  

---

## Audience

New engineers joining the Joinus Team working on the LinkedIn Job Applicants Exporter project (internal codename: ApplyPort).

---

## Purpose of This Document

This document explains:

- What the product is  
- Why it exists  
- What kind of system it is  

It intentionally avoids code-level or function-level details.

After reading this, a developer should understand:

- The problem being solved  
- The product philosophy  
- The type of data the system works with  
- The boundaries of responsibility  
- The long-term direction  

---

## 1. What This Product Is

LinkedIn Job Applicants Exporter (internally called ApplyPort) is a **browser-based hiring utility** that allows job posters on LinkedIn to extract and manage applicants from their own job posts.

It runs as a **Chrome extension** and operates entirely inside the user’s browser session.

At a high level, the product converts LinkedIn’s applicant pages into a **structured hiring workspace** where users can:

- Import applicants  
- View structured candidate profiles  
- Track basic hiring status  
- Export candidate data  

Think of the product as:

> A lightweight, local-first applicant tracking workspace embedded directly into LinkedIn.

---

## 2. Why This Product Exists

Many small companies and solo recruiters:

- Post jobs directly on LinkedIn  
- Do not use LinkedIn Recruiter  
- Do not use an ATS  

Yet they still need to:

- Collect applicant data  
- Organize candidates  
- Track basic hiring status  
- Export data into spreadsheets or tools  

Without this product, users rely on manual copy-paste and spreadsheets.

ApplyPort exists to remove this friction.

---

## 3. Product Philosophy

### Local-First
User data is stored locally in the browser by default.

### Zero-Friction
No login required.  
No onboarding flows.  
No account creation.

### Embedded Workflow
Users do not leave LinkedIn to use the product.

### User-Owned Data
Users control their data.  
The system does not sell or reuse applicant data.

---

## 4. What Kind of System This Is

ApplyPort is:

- A client-side Chrome extension  
- A data extraction layer  
- A local data management layer  
- A lightweight workflow layer  

ApplyPort is **not**:

- A traditional SaaS web app  
- A centralized backend-heavy system  
- A scraping infrastructure platform  

---

## 5. High-Level Data Flow (Conceptual)

1. User opens LinkedIn job applicants page  
2. LinkedIn loads applicant data  
3. ApplyPort observes existing data responses  
4. Data is structured into internal models  
5. Data is stored locally  
6. User interacts with the dataset  

The extension does not generate or fabricate data.  
It structures data already available to the job owner.

---

## 6. Types of Data the Product Works With

### Candidate Data

- Identity (name, photo, LinkedIn profile)  
- Contact information (email, phone when available)  
- Application metadata (date, position, company)  
- Screening questions and answers  
- Work experience  
- Education  
- Location  
- Internal status (new, shortlisted, under review, rejected)  
- Internal notes  

### Job Data

- Job title  
- Company  
- Location  
- Posting date  
- Candidate count  
- Job status  

---

## 7. Assumptions for Developers

- LinkedIn UI and data structures can change  
- Some data may be missing or partial  
- Performance matters (runs in-browser)  
- Privacy is a first-class constraint  
- Offline-friendly behavior is valuable  

---

## 8. Boundaries of Responsibility

ApplyPort:

- Structures applicant data  
- Stores and manages local records  
- Enables export  

ApplyPort does **not**:

- Decide hiring outcomes  
- Enrich data from third parties  
- Replace a full ATS  
- Circumvent LinkedIn authentication  

---

## 9. Current Product Stage

- Live on Chrome Web Store  
- Hundreds of active users  
- Core functionality stable  
- Monetization features emerging  

This is a production system.

---

## 10. Long-Term Direction

Potential evolution:

- Lightweight ATS  
- Data sync to hiring platforms  
- Collaboration features  

Core principle remains:

> Browser-native, recruiter-owned, privacy-first applicant management.

---

## 11. How to Think About Changes

When proposing or implementing features:

- Does this reduce friction?  
- Does this respect user data ownership?  
- Does this keep the product simple?  
- Does this work without requiring login?  

If not, reconsider.

---

## 12. Summary

LinkedIn Job Applicants Exporter is a Chrome-based, local-first hiring utility that converts LinkedIn applicant pages into structured, manageable candidate data.

Engineers working on this project are building infrastructure for **how hiring data is handled inside the browser**.
