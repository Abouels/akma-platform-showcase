# Operational workflows

This document outlines the key workflows orchestrated by the AKMA Platform. Each flow translates a real ‑world business process into a series of steps across modules. These flows ensure data consistency, enforce permissions and provide a traceable audit trail.

## Procurement cycle

The procurement module manages the end‑to‑end purchasing process:

1. **Purchase request** – A site engineer or project manager raises a purchase request for one or more BoQ items, specifying quantities and required dates. The request automatically references the relevant project and cost centre.
2. **Supplier comparison** – Procurement staff invite suppliers to submit offers, record received quotations and compare unit prices, delivery times and terms.
3. **Purchase order** – After selecting the best offer, the purchase request is converted into a purchase order. This order is approved by the authorised role (e.g. project manager or director).
4. **Goods receipt** – When materials arrive, warehouse staff record the received quantities against the purchase order. Any shortages or damages are noted. Inventory is updated in the warehousing module.
5. **Invoice & payment** – Supplier invoices are linked to the purchase order. The finance team reviews and approves invoices, schedules payments and records settlement.

This workflow enforces segregation of duties and supports multi‑currency, taxes and advance payments.

## Bill of Quantities (BoQ) lifecycle

The BoQ module governs how quantities and unit prices are defined and revised:

1. **BoQ creation** – For each project, an initial BoQ is created listing items, descriptions, units, quantities and unit prices. Projects may have multiple phases and associated BoQ sheets.
2. **Revision management** – Changes in scope or unit rates are managed via BoQ revisions. Previous revisions are preserved for audit. Approved revisions update budgets and procurement limits.
3. **Integration with procurement** – Purchase requests must reference BoQ items, ensuring that quantities ordered do not exceed the remaining quantities in the latest revision.
4. **Progress tracking** – As goods are received and consumed, the system updates delivered quantities, remaining quantities and cost variances for each BoQ item.

## Warehousing & inventory

The warehousing module tracks material movements and stock levels:

1. **Stock in** – Goods from purchase orders or returns are added to the appropriate warehouse. Each entry records batch numbers, expiry dates (if applicable) and storage locations.
2. **Stock out** – Materials issued to site or used in the project are deducted from warehouse stock. Users specify the consuming project and BoQ item, enabling cost allocation.
3. **Transfers** – Materials can be transferred between warehouses (e.g. from central store to site store), maintaining a traceable chain.
4. **Alerts & reordering** – Minimum stock levels trigger alerts to procurement. Users can generate suggested purchase requests based on reorder points and lead times.

## Finance & payments

The finance module provides a unified view of cash inflows and outflows:

1. **Income entries** – Record progress payments from clients, advances and other income. Each receipt references the project and can be allocated against specific BoQ items or milestones.
2. **Expense entries** – Capture direct expenses (materials, subcontractor bills), indirect expenses (salaries, rent) and miscellaneous charges. Each expense links to the relevant project, supplier invoice or purchase order.
3. **Invoice management** – Supplier invoices received via procurement are reviewed, approved and scheduled for payment. The system supports partial payments, retention amounts and withholdings.
4. **Cash flow reporting** – Users can generate cash flow statements by project or period, showing outstanding receivables, payables and available cash.

These workflows work together to give management real‑time visibility of costs, commitments and remaining budgets.
