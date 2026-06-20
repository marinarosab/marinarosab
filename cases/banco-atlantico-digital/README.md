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

Tribe Mission
SquadsAPP-Mobile - Build and evolve the bank's mobile app — the primary digital touchpoint for customersSquad Discovery (Upstream), Squad Delivery (Downstream), Squad Experience (UX)OpenBanking-APIBuild the bank's open connectivity layer, expose services to TPPs, and ensure secure authentication and platform infrastructureSquad Identidade, Squad Integrações, Squad PlataformaBackoffice-CreditoDigitise and automate internal credit processes, replacing legacy COBOL systems and paper-based workflowsSquad Automação, Squad Digitalização, Squad Integrações

## Regulatory Context

This simulation operates under real Portuguese and European regulatory constraints:

- PSD2 (Payment Services Directive 2): Requires BAD to expose open APIs to certified Third Party Providers (TPPs), covering Account Information Services (AIS) and Payment Initiation Services (PIS). Implemented by the OpenBanking-API tribe.
- GDPR / RGPD: Requires explicit consent management, the right to erasure, and full auditability of access to personal data. Embedded across OpenBanking-API and Backoffice-Credito backlogs.
- Banco de Portugal: Regulatory supervision context for TPP certification and credit process compliance.

These constraints are not decorative - they directly shape backlog prioritisation, Definition of Done, and acceptance criteria across all squads.

## PI2026Q2 - Backlog Overview

🏦 Tribe: APP-Mobile

The mobile app is the most visible layer of the transformation. Every capability built by the other tribes - open APIs, digitalised credit - ultimately reaches the customer through this channel.

Epic 1 · Gestão de Conta e Operações Diárias

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
