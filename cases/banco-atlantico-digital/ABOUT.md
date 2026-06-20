# 🏦 Case · Banco Atlântico Digital (BAD)

- Type: Side project / Simulation
- Tool: Azure DevOps
- Period: PI2026Q2 (April to June 2026)
- Role: Scrum Master & Agile Delivery

## Context

Banco Atlântico Digital (BAD) is a fictional Portuguese bank used as a simulation environment to practise and document agile delivery at scale.

The scenario: a traditional retail bank, founded in the 1980s, operating on COBOL-based legacy systems and paper-heavy processes. By 2026, the bank faces a convergence of pressures - regulatory deadlines (PSD2, GDPR), fintech competition eroding its younger customer base, and a new Chief Digital Officer mandated to accelerate the migration of core services to digital channels.

The board approves a transformation programme. Three tribes are formed. This is their first PI.

This project exists to simulate what it looks like to set up and facilitate agile delivery in a complex, regulated environment - with real backlog structure, real regulatory context, and real delivery decisions.

## Programme Structure

3 Tribes · 9 Squads · 1 PI · 6 Sprints

| Tribe | Mission | Squads |
|---|---|---|
| **APP-Mobile** | Build and evolve the bank's mobile app - the primary digital touchpoint for customers | Squad Discovery (Upstream), Squad Delivery (Downstream), Squad Experience (UX) | 
| **OpenBanking-API** | Build the bank's open connectivity layer, expose services to TPPs, and ensure secure authentication and platform infrastructure | Squad Identidade, Squad Integrações, Squad Plataforma | 
| **Backoffice-Credito** | Digitise and automate internal credit processes, replacing legacy COBOL systems and paper-based workflows | Squad Automação, Squad Digitalização, Squad Integrações |

## Regulatory Context

This simulation operates under real Portuguese and European regulatory constraints:

- PSD2 (Payment Services Directive 2): Requires BAD to expose open APIs to certified Third Party Providers (TPPs), covering Account Information Services (AIS) and Payment Initiation Services (PIS). Implemented by the OpenBanking-API tribe.
- GDPR / RGPD: Requires explicit consent management, the right to erasure, and full auditability of access to personal data. Embedded across OpenBanking-API and Backoffice-Credito backlogs.
- Banco de Portugal: Regulatory supervision context for TPP certification and credit process compliance.

These constraints are not decorative - they directly shape backlog prioritisation, Definition of Done, and acceptance criteria across all squads.

## PI2026Q2 - Backlog Overview

### **🏦 Tribe: APP-Mobile**

The mobile app is the most visible layer of the transformation. Every capability built by the other tribes - open APIs, digitalised credit - ultimately reaches the customer through this channel.

**Epic 1 · Gestão de Conta e Operações Diárias**

Feature: Dashboard Financeiro
- Real-time balance and transaction view
- Financial dashboard design (prototype + usability testing)
- PDF statement export

Feature: Transferências e Pagamentos
- SEPA transfers
- MB WAY payments and MB references

Feature: Notificações e Alertas
- Notification preference centre
- Push notification system

Feature: Acessibilidade
- WCAG 2.1 accessibility audit

**Epic 2 · Onboarding Digital sem Papel**

Feature: Registo e Validação de Identidade
- Onboarding journey map
- Welcome screen and initial registration flow
- Onboarding flow wireframes and prototype
- Identity document validation (CC / Passport)
- Liveness check (selfie validation)

Feature: Activação de Conta e Cartão
- PIN setup, biometric authentication and card view
- Account confirmation screen with simplified summary view

### **🔌 Tribe: OpenBanking-API**

This tribe exists because PSD2 makes it mandatory. Without a compliant open API layer, BAD cannot operate in the European payments ecosystem. The complexity here is not just technical - it requires alignment between legal, security, and product teams across multiple squads.

**Epic 1 · Conformidade PSD2 e Open Banking**

Feature: Gateway de APIs PSD2
- AIS endpoint (Account Information Service)
- PIS endpoint (Payment Initiation Service)
- External developer sandbox
- Rate limiting and API call logging
- Availability monitoring and alerts
- Load testing and final hardening

Feature: Portal Developer (DevPortal)
- Interactive API documentation (Swagger / OpenAPI)
- TPP application registration and management
- TPP credential self-service
- DevPortal usage analytics

**Epic 2 · Gestão de Identidade e Consentimentos**

Feature: Autenticação Forte (SCA)
- MFA for TPP access
- OAuth2 + PKCE flow
- Session and access token management

Feature: Centro de Consentimentos do Cliente
- Active consents dashboard
- Real-time consent revocation
- GDPR access audit report
- GDPR audit report exportable at PI close

### **🏛️ Tribe: Backoffice-Credito**

A personal credit application at BAD currently takes 5 to 10 business days - not because of underwriting complexity, but because of process inefficiency: physical documents circulating between departments, approvals by email, data entered manually into multiple disconnected systems. This tribe exists to eliminate exactly that.

**Epic 1 · Automação de Decisões e Workflows de Crédito**

Feature: Motor de Decisão de Crédito
Feature: Monitorização e Compliance Operacional
Feature: Integrações Regulatórias e de Segurança

**Epic 2 · Digitalização do Processo de Pedido de Crédito**

Feature: Digitalização do Processo de Pedido de Crédito
Feature: Integrações com Sistemas Legados e Canais Digitais

## Delivery Plan · PI2026Q2 · Visão Geral

6 sprints, 2 weeks each, running in parallel across all 3 tribes (April to June 2026).

| Sprint | Dates
|---|---| 
| Sprint 1 | 01/04 – 15/04 | 
| Sprint 2 | 16/04 – 30/04 | 
| Sprint 3 | 04/05 – 15/05 | 
| Sprint 4 | (continuing) |
| Sprint 5 | (continuing) | 
| Sprint 6 | (PI close) |

Each tribe runs its own squad-level ceremonies. Cross-tribe dependencies are managed through the Delivery Plan and flagged in the inter-sprint refinement sessions.

## Delivery Decisions & Backlog Rationale

**Why this prioritisation?**

The PI backlog was not assembled arbitrarily. Key decisions and the reasoning behind them:

OpenBanking-API leads on compliance, not features.
PSD2 has regulatory deadlines. 
The Gateway de APIs PSD2 and the identity/consent layer were placed in Sprint 1–2 to reduce regulatory risk early in the PI. 
Building the DevPortal in parallel enables TPP onboarding to begin before the PI closes.

APP-Mobile sequences by user impact.
Onboarding Digital sem Papel was prioritised alongside account management features because customer acquisition depends on it. 
A frictionless onboarding flow directly affects the bank's ability to grow its digital customer base - which is the business case for the entire transformation.

Backoffice-Credito attacks process waste, not just technology.
The credit automation epic targets the 5–10 day approval cycle. 
The decision to digitise the process before replacing the legacy systems (rather than the other way around) was deliberate: it reduces risk, allows parallel operation, and delivers visible improvement to internal teams faster.

**Dependency management**

The three tribes are not independent. 
APP-Mobile depends on OpenBanking-API for authentication flows. 
Backoffice-Credito depends on APP-Mobile for the customer-facing credit application journey. 
These dependencies are tracked in the Delivery Plan and flagged for inter-squad alignment at refinement.

## What's next in this project

- User Story breakdown for all PBIs
- Sprint Planning simulation for Sprint 1 (all 3 tribes)
- Definition of Ready (DoR) and Definition of Done (DoD) per tribe
- Team agreements per squad
- Retrospective artefacts at Sprint 2 close
- PI Review simulation at Sprint 6

## Process documents

| File | What is |
|---|---|
| dor.md | Definition of Ready |
| dod.md | Definition of Done |
| team-agreements.md | Team agreements |
| sprint-planning-sprint1.md | Sprint 1 Planning notes |

***Coming soon - being built incrementally alongside the Azure DevOps simulation.***

##Screenshots

| Description | File | 
|---|---|
| APP-Mobile backlog - Epic 1 | assets/app-mobile-backlog-epic1.png | 
| APP-Mobile backlog - Epic 2 | assets/app-mobile-backlog-epic2.png | 
| OpenBanking-API backlog - Epic 1 | assets/openbanking-backlog-epic1.png | 
| OpenBanking-API backlog — Epic 2 | assets/openbanking-backlog-epic2.png |
| Backoffice-Credito backlog | assets/backoffice-credito-backlog.png | 
| Delivery Plans list | assets/delivery-plans-list.png | 
Delivery Plan - PI2026Q2 Visão Geral | assets/delivery-plan-pi2026q2.png |

***This case is a living document - updated as the simulation progresses.***
