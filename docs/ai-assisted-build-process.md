# AI‑Assisted Build Process

### Introduction

This document describes how AI tools were leveraged to accelerate the design and prototyping of the AKMA platform. Prompt‑driven generative systems allowed us to rapidly translate business requirements into working prototypes, while human review ensured the outputs met the real needs of the project.

### Prompt engineering & specification

* Structured prompts were crafted to describe each module’s purpose, data fields, workflows and user interface expectations. Prompts included details on bilingual labels (Arabic/English), roles and permissions, and print requirements.
* Prompts were iteratively refined based on the AI‑generated outputs. When a generated screen or data structure did not align with the business logic, the prompt was adjusted to be more specific.

### Generating prototypes

* AI code generation tools were used to create initial versions of models, forms and lists for modules such as Projects, BoQs, Purchase Requests, Purchase Orders, Goods Receipts, Warehouses and Finance.
* Layout components and print templates were generated with basic styling to visualise how the data would appear on screen and on printed documents.

### Human review & iteration

* Each AI‑generated module was tested with dummy data to verify functionality. Issues such as missing fields, incorrect relationships or unintuitive navigation were noted.
* Prompts were updated or manual modifications were applied to the generated code to correct misalignments and to incorporate complex business rules (e.g. BoQ revision management, multi‑stage approvals).
* The human analyst ensured that data relationships, validations and process flows matched the company’s actual operations.

### Integrating modules

* AI‑generated modules were combined with manually written integration logic to connect workflows end‑to‑end. For example, converting a purchase request into a purchase order, or having goods receipts update warehouse stock and finance modules.
* Role‑based access checks and localisation functions were added to the generated code to enforce permissions and bilingual display.

### Limitations & considerations

* AI‑generated outputs required careful verification. The AI occasionally produced code that did not fully comply with business rules or that overlooked edge cases.
* Security, performance and data integrity considerations were addressed manually. Sensitive information and proprietary business logic are not included in this public showcase.

### Benefits

* Using AI prototypes accelerated early development stages, enabling rapid visualisation and validation of requirements with stakeholders.
* The process showcased skills in prompt engineering and systems analysis, highlighting the ability to direct AI tools towards meaningful outputs and to bridge the gap between business needs and technical implementation.

This AI‑assisted build process, combined with human expertise, was key to delivering a coherent and well‑aligned system design in a short timeframe.
