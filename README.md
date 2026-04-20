# AKMA Platform – AI‑Assisted Business System for Construction & Finishing Operations

The **AKMA Platform** is a case study in designing and building a business management system for the construction and finishing sector.  
It illustrates how a real business need was translated into a modular workflow-driven system, using prompt‑driven AI prototyping and iterative human review.  
The full production codebase is proprietary and owned by the sponsoring company, so it is **not included** here.  
This repository is instead a showcase of the system’s design, documentation and screenshots for portfolio and educational purposes.

## Why this system?

Small and medium‑sized contractors face common operational bottlenecks: scattered spreadsheets, manual procurement processes, poor visibility into costs and inventory and cumbersome reporting.  
AKMA addresses these pain‑points by offering a centralized system that covers projects, bills of quantities, procurement, warehousing, finance, permissions and reporting.  
The platform is multi‑lingual (Arabic and English) and enforces granular access control across roles such as administrators, project managers, procurement staff, accountants and consultants.

## Key Modules & Features

- **Projects & Accounts** – Create projects with detailed metadata, define accounts, and configure cost centers. Projects have statuses, phases and hierarchies.  
- **Bill of Quantities (BoQ)** – Generate structured BoQ tables, with categories, items, quantities, units and unit prices. Support for multiple projects and revisions.  
- **Procurement & Vendors** – Raise purchase requests, compare supplier offers, approve purchase orders, receive goods and manage supplier invoices.  
- **Warehousing & Inventory** – Track materials on site, record stock in/out, monitor remaining quantities and flag low stock levels.  
- **Finance & Payments** – Record income and expenses by project, link invoices, track advance payments, issue receipts and compile cash‑flow reports.  
- **Reporting & Printing** – Generate printable PDF reports (in Arabic/English), including project summaries, BoQ sheets, procurement comparisons, stock sheets and financial statements.  
- **Permissions & Multi‑Language** – Define user roles and group‑based permissions on each screen and action. The interface is fully bilingual.  
- **AI‑Assisted Prototyping** – Use generative AI to bootstrap initial prototypes, accelerate screen design and iterate rapidly based on user feedback.

## My Role

I acted as the **business systems analyst, product owner and AI prompt engineer** for this project. My responsibilities included:

- **Requirements elicitation** – Understanding the construction/finishing operations and translating them into system modules and workflows.  
- **Workflow definition** – Mapping real‑world processes (e.g. purchase request → supplier comparison → purchase order → receipt → invoice → payment) into system logic.  
- **Module & permission design** – Specifying the structure of each module, the fields needed and the roles that can view/edit data.  
- **UX and report direction** – Outlining dashboards, navigation patterns, Arabic/English labels, print layouts and data visualisations.  
- **AI‑assisted prototyping** – Leveraging generative models to scaffold screens and logic, then refining and validating outputs through iterative testing.  
- **Iteration & quality assurance** – Reviewing early builds, highlighting bugs and edge‑cases, and ensuring the final system met business expectations.

## Repository contents

This repository contains high‑level documentation and example artefacts:
- 
## Documentation

Detailed markdown files are provided in the `docs` folder to explain different aspects of the platform:

- [project-overview.md](docs/project-overview.md) – High-level summary of the system’s purpose, target users and benefits.
- [module-map.md](docs/module-map.md) – Overview of the key system modules (Projects, Procurement, Warehousing, Finance, Reporting) and how they relate to each other.
- [workflows.md](docs/workflows.md) – Detailed business processes covering the procurement cycle, BoQ lifecycle, warehouse management and finance operations.
- [roles-permissions.md](docs/roles-permissions.md) – Descriptions of the roles and a permissions matrix showing which roles can view/edit/approve data across modules.
- [reporting-printing.md](docs/reporting-printing.md) – Overview of reporting features, standard reports, print templates and export options.
- [version-history.md](docs/version-history.md) – Timeline of key milestones, features and iterations during the build of the platform.
- [ai-assist`d-build-process.md](docs/ai-assisted-build-process.md) – How generative AI tools were used to prototype and iterate on the system, and how human review ensured alignment with business needs.
- `screenshots/` – Placeholder folder for UI screenshots (e.g. dashboards, procurement flows). Real screens are excluded for confidentiality; you can add blurred or mock images here.  
- `assets/` – Static assets such as logos or icons.  

## Notes on confidentiality

The AKMA Platform is a commercial, proprietary system built for a real business context.  
**No production code or sensitive data is included** in this repository.  
The documentation and structures provided here are for demonstration and portfolio purposes only.  
If you wish to see a live demo or discuss licensing, please contact the author.
