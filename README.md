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

## Client Stakeholder Consultations

The primary objective of the stakeholder consultations was to develop a deep domain understanding of the client's business, identify operational pain points directly from personnel across multiple organizational levels, map core business processes, and get the answers to all relevant questions required to engineer an optimal solution design covering the needs and nuances of the client's business.

To ensure real-world analytical training, the roles of client stakeholders were simulated by our course instructors, **Ing. Jan Kočí, Ph.D.** and **Ing. Pavel Náplava, Ph.D.** In each session, they strictly maintained the realistic information scope, perspective, and operational domain knowledge of the assigned role, requiring our team to ask questions that were relevant to each interviewee's sphere of competence.

Each consultation followed a formal protocol: our team produced an advance preparation document (*Příprava na jednání*) outlining key topics and hypotheses, and concluded with an official meeting record (*Zápis z jednání*) to register the client's statements and requirements without subjective assumptions.

| Consultation | Client Stakeholder (Role) | Focus Area | Deliverables |
|:---|:---|:---|:---|
| **Consultation 1**<br>*(05.03.2026)* | **Commercial Director**<br>*(Jan Kočí)* | • Strategic vision, dealership network expansion history, and family-business governance<br>• Executive rationale for branch autonomy vs. systemic impact on profitability<br>• Commercial priorities, network-wide stagnation, and target transformation objectives | 📄 [Preparation Brief](uploads/0730-Priprava-AUTA-2026-03-05-1.pdf)<br>📝 [Meeting Record](uploads/0730-Zapis-AUTA-2026-03-05.pdf) |
| **Consultation 2**<br>*(12.03.2026)* | **Branch Manager (Ostrava)**<br>*(Jan Kočí)* | • Daily regional operations, local staff coordination, and branch autonomy limits<br>• Operational pain points: decentralized parts purchasing, lack of shared inventory, and scheduling friction<br>• Branch personnel digital readiness, change appetite, and local efficiency metrics | 📄 [Preparation Brief](uploads/0730-Priprava-AUTA-2026-03-12.pdf)<br>📝 [Meeting Record](uploads/0730-Zapis-AUTA-2026-03-12.pdf) |
| **Consultation 3**<br>*(26.03.2026)* | • **Service Advisor (Ostrava)**<br>*(Jan Kočí)*<br><br>• **Deputy Head of Sales (Ostrava)**<br>*(Pavel Náplava)* | • **Sales:** Dealership sales routines, B2B/B2C client tracking, and CRM customer profile needs<br>• **Service:** Frontline vehicle intake, repair booking friction, and customer communication bottlenecks<br>• **Workshop:** Diagnostic bay handoff, mechanic tablet interface requirements, and customer extra-work approval | 📄 [Preparation Brief](uploads/0730-Priprava-AUTA-2026-03-26.pdf)<br>📝 [Meeting Record](uploads/0730-Zapis-AUTA-2026-03-26.pdf) |
| **Consultation 4**<br>*(09.04.2026)* | **Branch Manager (Ostrava)**<br>*(Jan Kočí)* | • Practical review of TO-BE system architecture and proposed workflow feasibility at branch level<br>• Validation of technician incentive bonus formulas and workshop tablet integration<br>• Financial verification: local hardware budgeting, staff training rollout, and pilot deployment | 📄 [Preparation Brief](uploads/0730-Priprava-AUTA-2026-04-09.pdf)<br>📝 [Meeting Record](uploads/0730-Zapis-AUTA-2026-04-09.pdf) |

---

## <a id="is-solution-design"></a>IS Solution Design (Úvodní studie)

The **IS Solution Design (Úvodní studie)** represents the master deliverable and comprehensive final report of the project. It begins with a detailed baseline analysis of the client's current operational state, followed by a complete evaluation of all aspects of the proposed solution and its implementation — covering structural and architectural design, fulfillment of functional and non-functional requirements (FURPS+), project schedule, risk management, financial calculations.

📄 **Final Report Document (Full Master Deliverable):** [`Solution-Design-Report-Final.pdf`](Solution-Design-Report-Final.pdf)

---

### Report Structure

The complete study spans over 40 pages and is systematically structured into diagnostic, architectural, requirements engineering, schedule, risk, and financial chapters:

[![Solution Design Final Report - Contents](uploads/solution-design-final-report-contents.png)](uploads/solution-design-final-report-contents.png)

<p align="center"><em>Figure 2: Solution Design Final Report — Table of Contents</em></p>

---

### Key Highlights

#### SWOT Analysis and Strategy
Based on the conducted SWOT analysis, the project adopts a **MIN-MAX (Turnaround)** strategy. The evaluation revealed critical operational weaknesses across the dealership network — branch isolation, manual paperwork, and no centralized inventory or CRM — which directly threaten company profitability. The priority is to eliminate these internal bottlenecks first, establishing a solid operational baseline to capture market opportunities, improve margins, and strengthen competitive position:

[![SWOT Analysis](uploads/swot_analysis.png)](uploads/swot_analysis.png)

<p align="center"><em>Figure 3: SWOT Analysis Matrix — Global cars, a.s.</em></p>

<br>

#### Modular System Architecture
As our team is operating in the role of external IT contractor (**Enterprise Solutions, s.r.o.**), the proposed solution centers on the shipment of our company's established modular enterprise software product. The system architecture distinguishes between a standard **Core module package** included under the **baseline license** (highlighted in green in the diagram) and advanced functional modules licensed and delivered separately. Each module is customized to the client's operational workflows, with historical data migrated from existing legacy tools as needed. The final agreed modular architecture tailored to Global cars, a.s. is illustrated below:

[![Modular Architecture](uploads/module_architecture.png)](uploads/module_architecture.png)

<p align="center"><em>Figure 4: Proposed IS Modular Architecture (Core modules in green)</em></p>

<br>

#### Project Harmonogram
The project realization schedule is structured into distinct delivery phases: requirements mapping, system design, implementation, testing, staff training, branch rollout, and ongoing support. Each stage is scheduled around the client's operational capacity and designated availability windows, ensuring a seamless transition and minimal disruption to daily dealership operations. The schedule is illustrated in the Gantt chart below:

[![Project Harmonogram](uploads/project_harmonogram.png)](uploads/project_harmonogram.png)

<p align="center"><em>Figure 5: Project Realization Gantt Chart</em></p>

<br>

#### Financial Analysis

A comprehensive financial analysis model was constructed to evaluate project feasibility and return on investment. The calculation covers core software licensing, contractor implementation man-hours across delivery phases, ongoing support, and expected operational savings from optimized dealership and workshop business processes.

Presented below is the calculation table of man-hours required for module configuration tailored to the client's requirements across project phases, as a part of the complete financial analysis spreadsheet:

[![Module Configuration Man-Hours by Phase (Financial Model)](uploads/financial_analysis_core_manhours.png)](uploads/financial_analysis_core_manhours.png)

<p align="center"><em>Figure 6: Module Configuration Man-Hours by Phase (Part of the Complete Financial Analysis)</em></p>

📊 **Complete Financial Analysis Spreadsheet:** [`0730-CENIK-AUTA-2026-05-07.xlsx`](uploads/0730-CENIK-AUTA-2026-05-07.xlsx)

---

## <a id="process-engineering"></a><a id="process-mapping"></a>Process Engineering - BPMN 2.0

The reengineered vehicle service process features:

- Customer booking form with vehicle make/model, damage or requested service description, and photo upload.
- Intake technician interface to accept reservation requests or return them for clarification.
- CRM module with customer profiles and previous visit history.
- Critical ERP module to check and plan mechanic, parts, and equipment availability and offer available time slots.
- Spare parts ordering and inventory checks.
- Reservation dispatch to specific mechanics.
- Vehicle photo documentation upon intake at the workshop.
- Mechanic task assignments and timers to track efficiency and reward top performers.
- Dynamic order expansion sent directly to the customer for approval if extra repairs are needed.
- Loyalty program for returning customers.
- Post-service feedback form.
- And more.

The reengineered process is illustrated by the BPMN 2.0 chart below:

[![CLICK TO VIEW HIGH-RES](https://img.shields.io/badge/CLICK_TO_VIEW_HIGH--RES-555555?style=for-the-badge&logo=camunda&logoColor=FF6A00)](uploads/0730-ProcesniDiagram-AUTA-2026-05-21.png)
[![CAMUNDA MODELER](https://img.shields.io/badge/CAMUNDA_MODELER-FF6A00?style=for-the-badge)](https://modeler.camunda.io/share/8adf8ccf-61b5-4e5e-ac0b-5813c810a954)

[![Reengineered Process Model](uploads/0730-ProcesniDiagram-AUTA-2026-05-21.png)](uploads/0730-ProcesniDiagram-AUTA-2026-05-21.png)

<p align="center"><em>Figure 7: Reengineered Vehicle Service Process Model (BPMN 2.0)</em></p>


---
