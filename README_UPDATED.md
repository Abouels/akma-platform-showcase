# AKMA Platform – AI‑Assisted Business System for Construction & Finishing Operations

The **AKMA Platform** is a real‑world business system built for a finishing and general contracting company.  
It manages everything from clients and projects to procurement, inventory, finances, reports and internal support.  
This repository **does not include the production code**—it is a portfolio showcase of the system’s design, documentation and selected screenshots.  
The underlying implementation remains proprietary to the sponsoring company.

## Why this system?

Small and medium‑sized contractors often struggle with scattered spreadsheets, manual procurement, limited visibility into costs and cumbersome reporting.  
AKMA solves these bottlenecks by providing a **centralised, modular and bilingual platform** that connects all operational workflows in one place.  
It supports Arabic and English, enforces role‑based permissions, and is built to scale as the business grows.

## Core product direction

- **Project‑centric architecture** – every record is tied back to a project.  
- **Bilingual user interface** – full Arabic/English support with RTL/LTR switching.  
- **Role‑based access** – granular permissions per screen and action.  
- **Extensible modules** – new workflows can be added without breaking existing flows.  
- **Real operational and financial visibility** – dashboards and reports that reflect the current state of projects, budgets and inventory.  
- **Multi‑device web app** – responsive UI built with modern web technologies.  
- **Internal support & notifications** – helpdesk workflow and in‑app notifications instead of email‑only support.

## Main modules

1. **Clients** – profiles, contact details, markup settings and multi‑project relationships.  
2. **Projects** – workspace per client with metadata, dashboards, timelines and financial tracking.  
3. **Areas / Spaces** – rooms within each project with status and progress visibility.  
4. **Initial Handover** – track takeover status for finishing categories (plastering, electrical, plumbing, painting, flooring, ceilings, doors, aluminium, etc.).  
5. **Bill of Quantities (BoQ) / Estimation** – create estimation versions, plan costs, manage BoQ line items and generate print/export‑ready sheets.  
6. **Procurement** – item master, price timeline, supplier comparison, purchase workflow and residual materials tracking.  
7. **Finance** – supplier invoices, project expenses, company expenses, client revenues and cash‑flow reports.  
8. **Labor & Subcontractors** – assignment records, subcontractor tracking and payment follow‑up.  
9. **Reports & Export** – company and project reports with branded exports on company paper.  
10. **Internal Support** – helpdesk workflow and notification bell for IT support tickets and replies.

## Latest release: `akma V2.03.13`

The most recent release includes several important improvements:

- **Internal helpdesk direction** – support requests are now managed via an in‑app helpdesk rather than email.  
- **Notification bell** – users receive real‑time notifications when support tickets are created or responded to.  
- **Real progress tracking** – project and room progress are calculated from actual item statuses rather than fixed values.  
- **Login page refinement** – improved transparency on the login card and unified AKMA navy colour across the interface.  
- **In‑system mail configuration** – IT support email settings can be managed from within the system.  
- **Export enhancements** – cleaner PDF outputs, improved table clipping and fixed A4 printing with reduced distortion.  
- **Arabic/English UI fixes** – better RTL/LTR behaviour in the top bar and side bar.  
- **Business rules enforcement** – safe client deletion rules when linked projects exist, and residual stock zero‑state highlighting restored.

For a full history of changes, see the [`CHANGELOG.md`](CHANGELOG.md) file.

## Functional highlights

- **Real progress based on data** – project and room completion percentages are tied directly to the statuses of BoQ items and room elements.  
- **Branded export flows** – company‑branded reports and BoQ sheets ready for printing on official letterhead.  
- **Centralised operational records** – all procurement, inventory, financial and labor data live in one database.  
- **AI‑assisted prototyping** – generative models were used to bootstrap screens and workflows, accelerating design and iteration.  
- **Multi‑language interface** – Arabic and English can be switched instantly without reloading.  
- **Built‑in helpdesk** – users can open support tickets and receive responses via the in‑app notification bell.

## Tech stack

- **Next.js 15** (React)  
- **TypeScript**  
- **Prisma ORM**  
- **PostgreSQL**  
- **Tailwind CSS**

## My role

I served as the **business systems analyst, product owner and AI prompt engineer** for the AKMA Platform.  
My responsibilities included:

- **Requirements elicitation** – understanding construction and finishing operations and translating them into modules and workflows.  
- **Workflow definition** – mapping real‑world processes (e.g. purchase request → supplier comparison → purchase order → receipt → invoice → payment) into system logic.  
- **Module & permission design** – specifying the structure of each module, the fields needed and the roles that can view/edit data.  
- **UX and report direction** – outlining dashboards, navigation patterns, bilingual labels, print layouts and data visualisations.  
- **AI‑assisted prototyping** – leveraging generative models to scaffold screens and logic, then refining and validating outputs through iterative testing.  
- **Iteration & quality assurance** – reviewing early builds, identifying bugs and edge cases, and ensuring the final system met business expectations.

## Versioning

Versions follow the pattern:

```
akma V<major>.<minor>.<patch>
```

For example, `akma V2.03.13` corresponds to **major version 2**, **minor version 3** and **patch release 13**. See `VERSIONING_RULES.md` for guidelines on incrementing these numbers.

## Repository contents

This repository contains high‑level documentation and artefacts:

- `docs/` – markdown documents explaining the system overview, module map, workflows, roles and permissions, reporting, version history and the AI‑assisted build process.  
- `docs/screenshots/` – screenshots of the UI (login, dashboard, projects, areas, BoQ, procurement, finance, reports, IT support). The actual image files should be added here when publishing this repo.  
- `assets/` – static assets such as logos or icons.  
- `CHANGELOG.md` – chronological list of changes across versions.  
- `RELEASE_TEMPLATE.md` – template for drafting future release notes.  
- `VERSIONING_RULES.md` – rules for determining version numbers.  
- `GITHUB_UPLOAD_STEPS.md` – instructions on how to prepare and upload new releases to GitHub.

## Documentation

Detailed documentation is provided in the `docs` folder:

- **[Project overview](docs/project-overview.md)** – background, purpose, target users and benefits of the system.  
- **[Module map](docs/module-map.md)** – table showing each module and how they relate to each other.  
- **[Workflows](docs/workflows.md)** – step‑by‑step descriptions of procurement, BoQ lifecycle, warehousing/inventory and finance/payment processes.  
- **[Roles & permissions](docs/roles-permissions.md)** – breakdown of user roles (admin, project manager, procurement officer, store manager, accountant, viewer/consultant) and the permissions granted in each module.  
- **[Reporting & printing](docs/reporting-printing.md)** – overview of standard reports, print templates and export options.  
- **[Version history](docs/version-history.md)** – log of releases and the key features added in each version.  
- **[AI‑assisted build process](docs/ai-assisted-build-process.md)** – explains how AI was used to generate prototypes and accelerate development.

## Screenshots

To make the README more vivid, add images under `docs/screenshots/` and link them here using the following file names:

| Screen                      | File name                             | Description                                             |
|----------------------------|---------------------------------------|---------------------------------------------------------|
| Login page                 | `login-page.png`                      | Shows the login card, background and branding.          |
| Company dashboard          | `company-dashboard.png`               | High‑level overview of projects, finances and KPIs.     |
| Projects list              | `projects-list.png`                   | List of all projects with quick access and summary.     |
| Project overview           | `project-overview.png`                | Details of a single project with progress indicators.   |
| Areas / Rooms              | `areas-rooms.png`                     | Room‑level status and progress within a project.        |
| Initial handover           | `initial-handover.png`                | Form showing initial handover statuses by category.     |
| BOQ / Estimation           | `boq-estimation.png`                  | Bill of Quantities table with quantities and costs.     |
| Procurement                | `procurement.png`                     | Supplier comparison and purchase workflow.             |
| Invoices & expenses        | `invoices-expenses.png`               | Screens for supplier invoices and company expenses.     |
| Reports                    | `reports.png`                         | Examples of reports and export previews.                |
| Internal IT support        | `it-support.png`                      | Helpdesk interface with tickets and notification bell. |

Optional extra images (if available) include clients, suppliers comparison, residual inventory, settings/users/roles and branded PDF exports.  
Remember to blur or remove any sensitive company data before publishing screenshots.

## Local setup (optional)

If you have access to the codebase, you can run the platform locally:

```bash
npm install
npx prisma generate
npx prisma migrate dev
npm run dev
```

Note that this repository does not contain the application source; the above steps are provided for completeness only.

## Notes on confidentiality

The AKMA Platform is a commercial system built for a real business context.  
This repository is a portfolio showcase of its design and documentation; **no production code or sensitive data are included**.  
Please contact the author for a private demo or licensing discussions.
