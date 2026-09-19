# Global cars, a.s. - Information System Solution Design

> **Institution:** CTU FEE (ČVUT FEL) | **Course:** B6B16INS (Information Systems)  
> 
> **Project:** Comprehensive IS solution design for the Global cars, a.s. dealership network in the Czech Republic.  
> 
> **Key competencies:** IT analytics, client meetings, process mapping, BPMN 2.0, functional prototype delivery, product ownership, client presentations, ERP, CRM, IS design, modular IS shipment and licensing.  
> 
> **Language:** Czech (Project deliverables) / English (Portfolio overview)

---

## Contents

1. [Business Case](#business-case)
   - [AS-IS Operational Reality and Company Profile](#as-is-operational-reality-and-company-profile)
   - [Business Model Canvas (BMC)](#business-model-canvas-bmc)
   - [Project Charter — Document A4](#project-charter--document-a4)
2. [Client Stakeholder Consultations](#client-stakeholder-consultations)
3. [IS Solution Design (Úvodní studie)](#is-solution-design)
   - [Report Structure](#report-structure)
   - [Key Highlights](#key-highlights)
4. [Process Engineering - BPMN 2.0](#process-engineering)
5. [Functional Prototype](#functional-prototype)
6. [Team Working Environment Logs – GitLab Wiki Pages (CZ)](#team-working-environment-logs--gitlab-wiki-pages)
   - [Projektový tým a role](#projektový-tým-a-role)
   - [Rizika projektu](#rizika-projektu)
   - [Evidence odpracovaných hodin a úkolů](#evidence-odpracovaných-hodin-a-úkolů)
   - [Závěrečné hodnocení členů týmu](#závěrečné-hodnocení-členů-týmu)
7. [Authors](#authors)

---

## Business Case

The initial business context, client operational baseline, and project assignment are defined in the university task specification:
- 📄 **University Assignment Document (Karta zákazníka):** [`Business-Case.pdf`](Business-Case.pdf) <br> *(original Czech assignment brief from CTU FEE)*

---

### AS-IS Operational Reality and Company Profile

**Global cars, a.s.** is a Czech automotive company operating an authorized dealership and service network for **Hyundai** passenger vehicles (sales, maintenance/repairs, and auxiliary short-term car rental). Headquartered in Prague (with registered capital of CZK 2,000,000 and approximately 80 employees), the company grew rapidly through acquisitions:
- **Network Expansion & Ownership:** Established two years prior through the acquisition of 6 dealerships (*Praha, Plzeň, Pardubice, Liberec, Tábor, Jihlava*), the network subsequently expanded to 9 branches across the Czech Republic by acquiring additional locations in *Brno, Olomouc, and Ostrava*. The business is 100% owned by a single private investor who funded the acquisition with capital gained from stock market investments. Management resides at the Prague headquarters and consists primarily of the owner's family members, operating the enterprise on a family-business model.
- **Core Operations vs. Auxiliary Activities:** Primary business revenue is driven by new and pre-owned vehicle sales and authorized vehicle service. Vehicle rental is run purely as a complementary service.

#### Structural Bottlenecks & AS-IS Deficiencies:
- **Operational Fragmentation Across Branches:** Following the rapid acquisition wave, all 9 branches continued to function completely autonomously. Each dealership maintained disparate local workflows, separate uncoordinated local suppliers for spare parts and shop supplies, and disconnected legacy software tools. There was no central data exchange, shared vehicle service history, or cross-branch inventory visibility.
- **Neglected ICT Infrastructure:** Executive leadership and local branch managers traditionally placed paramount emphasis on face-to-face customer relationships, priding themselves on above-standard personal customer care. Due to this mindset, systemic ICT development was heavily neglected. The company had no unified website, no central Customer Relationship Management (CRM) system, and no digital reservation or self-service scheduling platform.
- **Economic Vulnerability:** In the face of macroeconomic stagnation and rising operational overhead, the lack of centralized oversight, duplicated administrative work, and inefficient vehicle service scheduling began severely depressing profit margins and threatening the firm's financial sustainability.

---

### Business Model Canvas (BMC)

To systematically evaluate the company's business model and align strategic requirements, the **Business Model Canvas (BMC)** methodology was applied. It provides a structured evaluation across 9 fundamental blocks: Key Partners, Key Activities, Key Resources, Value Propositions, Customer Relationships, Channels, Customer Segments, Cost Structures, and Revenue Streams.

[![Business Model Canvas](uploads/0730-BMC-AUTA-2026-03-18.jpg)](uploads/0730-BMC-AUTA-2026-03-18.jpg)

<p align="center"><em>Figure 1: Business Model Canvas — Global cars, a.s.</em></p>

- 📄 **Business Model Canvas Document (PDF):** [`0730-BMC-AUTA-2026-03-18.pdf`](uploads/0730-BMC-AUTA-2026-03-18.pdf)

---

### Project Charter — Document A4

The **Document A4** is the initial project charter and business proposal delivered to the client, **Global cars, a.s.** 

Within the project, our team operated in the role of **Enterprise Solutions, s.r.o.** — an external IT contractor specializing in custom enterprise software development and systems modernization (*vývoj a modernizace IS na klíč*). The document establishes the project scope, bilateral business motivations, resource constraints, and executive governance prior to commencing detailed analytical work:
- **Problem Statement & Scope:** Formal mandate to overcome operational fragmentation across branches and design a centralized, process-unified IS solution spanning dealership sales and service bay management.
- **Client & Contractor Motivations:**
  - *Client Motivation:* Halting economic stagnation, modernizing business operations in line with contemporary industry standards, and interconnecting all 9 branches through a unified Information System.
  - *Contractor Motivation:* Entering the automotive enterprise IT domain, acquiring an authoritative industry reference, and expanding analytical and architectural competencies of their team.
- **Acceptance Criteria & Delivery Constraints:**
  - The fact of the client's sign-off on the target conceptual solution (*Úvodní studie*) that demonstrably and logically solves identified operational bottlenecks.
  - Strict compliance with delivery milestones and schedule.
  - Human resource and cost ceiling: 5-member contractor analytical team capped at a maximum of **300 billable man-hours** (total contract price of CZK 300,000 at CZK 1,000/hour; internal contractor team costs of CZK 225,000; 20 client consultation hours).
- **Steering Committee & Stakeholder Governance:** Establishes the joint executive steering committee (*Řídící komise*) consisting of client leadership sponsors (Commercial Director Jan Kočí, Sales Representative Pavel Náplava) and contractor leadership (Project Manager Mykhailo Plokhin, Lead Analyst Ivan Shestachenko).

📄 **Project Charter (Document A4):** [`0730-A4-AUTA-2026-03-03.pdf`](uploads/0730-A4-AUTA-2026-03-03.pdf)

---

