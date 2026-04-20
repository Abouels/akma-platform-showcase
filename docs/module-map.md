# Module map

This document summarises the major modules in the AKMA Platform and how they interrelate.

## Core modules

| Module | Description | Key entities |
|-------|------------|--------------|
| **Projects & accounts** | Define projects (site, client, start/end dates, budgets) and account structures. Projects form the root for all other data. | Projects, accounts, cost centres |
| **Bill of Quantities (BoQ)** | Structured list of tasks, materials and labour required for each project. Each BoQ item records quantity, unit, unit price and total cost. | BoQ, categories, items, units |
| **Procurement** | Manages the purchasing lifecycle from request to supplier selection to order issuance and receipt. | Purchase requests, suppliers/vendors, supplier offers, purchase orders, goods receipts |
| **Warehousing** | Tracks stock on site and in storage. Supports stock in/out transactions, minimum stock alerts and valuation. | Warehouses, stock items, stock transactions |
| **Finance** | Handles income and expenses for each project. Integrates with procurement and warehousing to reflect actual costs. | Income entries, expense entries, invoices, receipts, payments |
| **Reporting & printing** | Generates dashboards and printable reports across modules. Supports Arabic and English print templates. | Dashboards, PDF reports, exports |
| **Permissions & roles** | Centralised access control system defining what each user type can view or edit. | Roles, groups, permissions |

## Relationships

- Projects are the parent entity. Every BoQ, procurement request and financial entry belongs to a project.  
- BoQ items link to procurement requests. When a procurement request is created, it references the BoQ item(s) being purchased and their quantities.  
- Purchase requests generate multiple supplier offers. Approved offers convert to purchase orders. Purchase orders link to goods receipts once materials arrive.  
- Stock transactions update the warehousing module and feed into cost calculations.  
- Income and expense entries reference projects and sometimes specific BoQ items. These entries feed into financial reports.  
- Permissions are enforced at the module level and sometimes at the field/action level; for example, warehouse staff can create stock transactions but cannot view finance reports.
