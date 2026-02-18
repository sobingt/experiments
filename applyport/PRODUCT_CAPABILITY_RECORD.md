# 📘 Product Capability Record (PCR)

## Product Name
LinkedIn Job Applicants Exporter  

## Internal Codename
ApplyPort  

## Owner
Joinus Team  

## Distribution
Chrome Web Store  

## Product Category
- Hiring Productivity Tool  
- Lightweight Local ATS  
- LinkedIn Applicant Data Exporter  

## Product Status
Live – Production  

## Active Usage
400+ active users  

---

## 1. Product Overview

LinkedIn Job Applicants Exporter is a Chrome extension that enables LinkedIn job posters to extract, organize, track, and export applicants from their own LinkedIn job postings.

The product operates entirely inside the user’s browser and stores data locally by default.

---

## 2. Primary Use Cases

- Export LinkedIn applicants into CSV or JSON  
- Maintain a local candidate database  
- Track candidate status per job  
- View screening question answers  
- Share candidate data via exported files  

---

## 3. Supported LinkedIn Surfaces

Supported:

- Standard LinkedIn job posts created from LinkedIn dashboard  
- Applicants page for those jobs  

Not Supported:

- LinkedIn Recruiter  
- Third-party ATS views  

Only job owners/posters can use the product.

---

## 4. System Architecture

- Client-side Chrome extension  
- No backend required for core features  
- Uses LinkedIn’s existing network responses  
- Local browser storage  

Optional integrations:

- Google Sheets (planned)  
- Joinus.team platform (planned)  

---

## 5. Data Objects

### Candidate Object

- Full name  
- Profile photo  
- LinkedIn profile URL  
- Email address  
- Phone number  
- Location  
- Current job title  
- Current company  
- Past experience  
- Education history  
- Skills (if available)  
- Screening questions  
- Screening answers  
- Application date  
- Experience level  
- Connection status  
- Viewed-by-recruiter timestamp  
- Internal notes  
- Internal status  

### Job Object

- Job title  
- Company name  
- Location  
- Posting date  
- Total applicants  
- Job status  

---

## 6. Candidate Management Capabilities

- Candidate list view  
- Candidate detail view  
- Search candidates  
- View screening Q&A  
- Add notes  
- Update status (New, Shortlisted, Under Review, Rejected)  

---

## 7. Job Management Capabilities

- View all imported jobs  
- View per-job candidate counts  
- View per-job status summary  
- Open original LinkedIn job  

---

## 8. Export Capabilities

- Export candidates as CSV  
- Export candidates as JSON  
- Export all data from Settings  

Planned:

- Google Sheets export  
- Joinus.team sync  

---

## 9. Dashboard Capabilities

- Jobs processed  
- Candidates tracked  
- Exports completed  
- Days active  
- Storage utilization  
- Data size by category  

---

## 10. Settings & Data Management

- Export local data  
- Import local data (disabled currently)  
- Clear all local data  
- Premium feature gating  

---

## 11. Feedback & Support

- In-product feedback form  
- Star rating  
- Optional email capture  
- External support links  

---

## 12. Authentication

None required.

---

## 13. Pricing (Current)

Free

---

## 14. Compliance & Responsibility

- Users access only their own job applicant data  
- Data stored locally  
- No data resale  
- User responsible for compliance with local laws  

---

## 15. Known Limitations

- No LinkedIn Recruiter support  
- No team collaboration  
- No cross-job deduplication  
- No cloud backup  

---

## 16. Differentiators

- Works without LinkedIn Recruiter  
- Local-first  
- No login  
- Screening question extraction  
- Lightweight ATS behavior  

---

## 17. Product Maturity

Validated utility with real users and production usage.

---

## 18. One-Line Description

A local-first Chrome extension that turns LinkedIn job applicants into a structured, exportable hiring workspace.

---
