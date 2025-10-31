# 🌐 Oracle Fusion — Global Human Resources (Global HR / Core HR)

> README for **Global HR / Core HR** configuration and core HR transactions implemented in **Oracle Fusion HCM**.  
> This document lists configuration tasks, explains their purpose and responsibilities, and provides reference links to Oracle documentation.

---

## 📘 Overview

**Global Human Resources (Global HR / Core HR)** in Oracle Fusion forms the foundation for workforce management.  
It defines enterprise structures, legal and payroll entities, workforce classifications (jobs, positions, grades), and shared reference data required for HR, payroll, and talent processes.  

Use these configurations to model your organization for:
- Accurate HR reporting  
- Seamless payroll integration  
- Statutory compliance  
- Standardized employee management  

([docs.oracle.com][1])

---

## ⚙️ Configuration Checklist

Below are the configuration tasks (task name → setup summary).  
Perform these in **Setup and Maintenance** (*Global HR* or *Absence Management* work area) or via the **Enterprise Structures Configurator** where applicable.

1. **Geographies** — *Manage Geographies*  
   Define country/region/city hierarchies and validate geography lookups. Used for address, tax, and legal reporting. ([docs.oracle.com][2])

2. **Enterprise Structure** — *Establish Enterprise Structure*  
   Use the Enterprise Structure Configurator to create divisions, legal entities, business units, and reference data sets. Forms the core hierarchy for HR operations. ([docs.oracle.com][3])

3. **Enterprise HCM Information** — *Manage Enterprise HCM Information*  
   Maintain enterprise-level defaults and HCM settings shared across modules. ([docs.oracle.com][4])

4. **Reference Data Sets** — *Manage Reference Data Sets*  
   Create reusable reference data sets for lookups and configuration reuse across business units.

5. **Locations** — *Manage Locations*  
   Define physical office/worksite locations used in person, job, and assignment data.

6. **Divisions** — *Manage Divisions*  
   Define divisions to group business units and legal entities for enterprise reporting.

7. **Legal Address** — *Manage Legal Address*  
   Maintain official addresses used in legal and statutory documents.

8. **Legal Entity** — *Manage Legal Entity*  
   Create legal entities (companies registered under law). ([docs.oracle.com][5])

9. **Payroll Statutory Unit (PSU)** — *Manage Legal Entity / Payroll Statutory Unit*  
   Define payroll statutory units (tax reporting units) and associate legislative data groups. ([docs.oracle.com][6])

10. **Legal Employers** — *Manage Legal Employer*  
    Designate legal entities as employers responsible for employee relationships and payroll.

11. **Legal Entity HCM Information** — *Manage Legal Entity HCM Information*  
    Maintain HCM-specific data for legal entities (e.g., employer settings, payroll groupings). ([docs.oracle.com][7])

12. **Actions** — *Manage Actions*  
    Configure HR actions (Hire, Transfer, Promotion, Termination) and define how they trigger processes.

13. **Action Reasons** — *Manage Action Reasons*  
    Add standardized reasons (e.g., promotion → merit, termination → resignation) for reporting consistency.

14. **Lookups** — *Manage Lookups*  
    Define lookup types and values used across Core HR modules. ([docs.oracle.com][3])

15. **DFFs (Descriptive Flexfields)** — *Manage Descriptive Flexfields*  
    Extend Core HR tables to capture additional attributes not available by default.

16. **Business Units (BUs)** — *Manage Business Units*  
    Set up business units for managing transactions (HR, Payroll, Procurement).

17. **Assign Set IDs for Business Units** — *Manage Business Unit Set Assignment*  
    Map BUs to data sets (e.g., ledger or reference data set) for consistency.

18. **Departments** — *Manage Departments*  
    Create departments that define your organization’s reporting and management structure.

19. **Department Trees** — *Manage Department Trees*  
    Build hierarchical trees for approvals and organizational visualization.

20. **Grades** — *Manage Grades*  
    Define grade structures used for pay, job classification, and career progression.

21. **Grade Rates** — *Manage Grade Rates*  
    Associate pay ranges or rates with grades.

22. **Grade Ladders** — *Manage Grade Ladders*  
    Define grade progression paths (career advancement frameworks).

23. **Jobs** — *Manage Jobs*  
    Create generic job roles used for reporting, requisitioning, and assignments.

24. **Positions** — *Manage Positions*  
    Define specific position records linked to jobs and departments; supports headcount control.

25. **Position Trees** — *Manage Position Trees*  
    Build position hierarchies for workflow approvals and reporting.

26. **Person Types** — *Manage Person Types*  
    Define categories of people (Employee, Contingent Worker, Ex-Employee).

27. **Assignment Statuses** — *Manage Assignment Status*  
    Maintain status values (Active, Suspended, Terminated) for employee assignments.

---

## 🔄 Common Transactions / Core HR Operations

Once configuration is complete, you can perform these key **Global HR / Core HR transactions**:

* **Manage Person Name Styles** — Configure display formats for person names.  
* **Hire Employee** — Create a new person record, primary assignment, and legal employment. ([docs.oracle.com][8])  
* **Transfer Employee** — Move an employee between BUs, divisions, or legal entities. ([docs.oracle.com][9])  
* **Promotion** — Update job, grade, or compensation details.  
* **Termination** — End employment and finalize payroll and statutory data. ([docs.oracle.com][9])

---

## ✅ Implementation Notes & Best Practices

* Use **Enterprise Structures Configurator (ESC)** to define the full enterprise structure in one guided flow. ([docs.oracle.com][3])  
* Configure **Geographies** first — many validations depend on geography setup. ([docs.oracle.com][2])  
* Always associate **Legislative Data Groups** to PSUs for statutory compliance. ([docs.oracle.com][6])  
* Keep **DFFs** well-documented and minimal to maintain data integrity.  
* Maintain naming standards for Jobs, Positions, and Departments for easier reporting and integration.

---

## 📚 References

* Oracle — Overview of Global Human Resources. ([docs.oracle.com][1])  
* Oracle — Manage Geographies / Geography Structures. ([docs.oracle.com][2])  
* Oracle — Define Enterprise Structures for HCM. ([docs.oracle.com][3])  
* Oracle — Enterprise HCM Information Setup. ([docs.oracle.com][4])  
* Oracle — Creating Legal Entities using ESC. ([docs.oracle.com][5])  
* Oracle — Define Payroll Statutory Units and Legal Employers. ([docs.oracle.com][6])  
* Oracle — Global HR Implementation Guide. ([docs.oracle.com][10])

---

## ✍️ Author

**Rohit Anand**  
📍 Bangalore, India  
💼 Oracle HCM Functional Consultant

---

[1]: https://docs.oracle.com/en/cloud/saas/human-resources/24d/faigh/overview-of-global-human-resources.html?utm_source=chatgpt.com "Overview of Global Human Resources"
[2]: https://docs.oracle.com/en/cloud/saas/human-resources/faucf/manage-geography-structures-hierarchies-and-validation.html?utm_source=chatgpt.com "Manage Geography Structures and Hierarchies"
[3]: https://docs.oracle.com/cd/E15586_01/fusionapps.1111/e20380/F509848AN11B52.htm?utm_source=chatgpt.com "Define Enterprise Structures for Human Capital Management"
[4]: https://docs.oracle.com/en/cloud/saas/human-resources/faigh/overview-of-implementing-global-human-resources.html?utm_source=chatgpt.com "Implementing Global Human Resources"
[5]: https://docs.oracle.com/en/cloud/saas/human-resources/24d/faigh/how-you-create-legal-entities-in-the-enterprise-structures.html?utm_source=chatgpt.com "How You Create Legal Entities in the Enterprise Structures"
[6]: https://docs.oracle.com/en/cloud/saas/human-resources/fapuk/how-to-define-hcm-enterprise-structures-for-the-uk.html?utm_source=chatgpt.com "Define HCM Enterprise Structures"
[7]: https://docs.oracle.com/en/cloud/saas/human-resources/faigh/how-you-configure-your-enterprise-structure-after-an-acquisition.html?utm_source=chatgpt.com "Configure Enterprise Structure After Acquisition"
[8]: https://docs.oracle.com/en/cloud/saas/human-resources/24d/fawhr/using-global-human-resources.pdf?utm_source=chatgpt.com "Using Global Human Resources"
[9]: https://docs.oracle.com/cd/E51367_01/globalop_gs/FAWHR/FAWHR.pdf?utm_source=chatgpt.com "Oracle Global Human Resources Cloud Using Guide"
[10]: https://docs.oracle.com/en/cloud/saas/human-resources/24d/faigh/implementing-global-human-resources.pdf?utm_source=chatgpt.com "Implementing Global Human Resources"

---

## 📝 Points to Remember

* Please **clone the project** instead of downloading individual files.  
* Cloning or downloading the **entire repository as a ZIP** will include all required folders and images.  
* After downloading, **unzip the project** — you’ll find all the **execution screenshots** inside the designated folder (e.g., `/screenshots/`).  
* The images may not open correctly if viewed through “Download Raw” on GitHub — this is expected.  
* Always open images **locally after extraction** to view the execution results clearly.

---



