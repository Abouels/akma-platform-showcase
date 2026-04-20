# Roles & Permissions

### Purpose

This document defines typical user roles and the permissions assigned to each role within the AKMA platform. A clearly defined access-control model ensures that users only see and modify data relevant to their responsibilities and helps maintain data integrity and segregation of duties.

### Role descriptions

**Administrator** — This is the highest-level user role. Administrators can manage system configuration, create and delete users, assign roles and permissions, and have full read/write access across all modules and data. They can view and modify settings, module definitions, and reports.

**Project Manager** — Project managers are responsible for creating and managing projects and bills of quantities (BoQs). They can track project progress, monitor budgets versus actuals, review and approve purchase requests, and view procurement, warehouse and finance data. They cannot edit user accounts or system settings.

**Procurement Officer** — Procurement officers handle the end‑to‑end purchasing process. They create purchase requests, compare suppliers, issue purchase orders, record goods receipts and handle supplier invoices. They can view project budgets and BoQ items but cannot modify financial entries or manage user accounts.

**Warehouse Manager** — Warehouse managers oversee warehouse operations. They receive stock into warehouses, record stock issues, execute transfers between stores and manage current inventory levels. They can view purchase orders and BoQ items but cannot issue procurement orders or record financial transactions.

**Accountant / Finance** — Finance users manage cash inflows and outflows. They enter expense and income receipts, approve supplier invoices, record payments and generate financial reports. They can view procurement and warehouse entries but cannot modify them.

**Viewer / Consultant** — Viewers (consultants, auditors or clients) have read‑only access. They can view dashboards and reports but cannot create, edit or approve any data.

### Permissions matrix

The table below summarizes the high‑level permissions for each role across the main platform modules:

| Module / Function              | Administrator | Project Manager | Procurement Officer | Warehouse Manager | Accountant/Finance | Viewer |
|-------------------------------|--------------|----------------|--------------------|------------------|-------------------|--------|
| **User & Role Management**    | full         | none           | none               | none             | none              | none   |
| **Projects & BoQs**           | full         | create/edit    | view               | view             | view              | view   |
| **Procurement cycle**         | full         | approve        | create/edit        | view             | view              | view   |
| **Warehouse & Inventory**     | full         | view           | view               | create/edit      | view              | view   |
| **Finance & Payments**        | full         | view           | view               | view             | create/edit       | view   |
| **Reports & Dashboards**      | full         | view           | view               | view             | view              | view   |

*full* – can view, create, edit and delete records.  
*create/edit* – can create and modify records but not delete.  
*view* – read‑only access; cannot create or modify.  
*approve* – can approve requests within the module.  
*none* – no access.

These roles and permissions can be adapted to fit different company structures. The Administrator can customize roles or create new ones to suit the organization’s policies.
