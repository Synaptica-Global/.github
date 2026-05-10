<div align="center">

<img src="https://img.shields.io/badge/XIEM-Trade%20Compliance%20%26%20Procurement-1a3a6b?style=for-the-badge&labelColor=0a1628" alt="XIEM Platform"/>

# Synaptica Global

**AI-powered Trade Compliance & Procurement Platform for the GCC**

[![Platform](https://img.shields.io/badge/Platform-XIEM-1a3a6b?style=flat-square)](https://github.com/Synaptica-Global)
[![Region](https://img.shields.io/badge/Region-GCC-006c35?style=flat-square)](#)
[![Phase](https://img.shields.io/badge/Phase-KSA%20Construction-c8a951?style=flat-square)](#)
[![Repos](https://img.shields.io/badge/Repositories-25-1a3a6b?style=flat-square)](#)
[![Stack](https://img.shields.io/badge/Stack-TypeScript%20%7C%20Node.js%20%7C%20React%20%7C%20Docker-3178c6?style=flat-square)](#)

</div>

---

## What is XIEM?

XIEM is a multi-country, multi-vertical SaaS platform that automates trade compliance and procurement workflows across the GCC. It handles HS code classification, customs declarations, supplier management, VAT/duty calculations, ZATCA e-invoicing, SABER/SASO certification, FASAH shipment tracking, and municipality permit verification — all in one platform.

**Phase 1 — KSA Construction vertical is live.**

---

## Repository Structure

The platform is built on a 3-layer architecture with full isolation between countries and industry verticals.

### Layer 1 — Platform Core
Shared infrastructure used by all countries and verticals.

| Repository | Description |
|------------|-------------|
| [xiem-shared-types](../../xiem-shared-types) | Shared TypeScript types and interfaces |
| [xiem-api-gateway](../../xiem-api-gateway) | Single entry point routing to all services |
| [xiem-infra-config](../../xiem-infra-config) | Docker Compose, environment, database configuration |
| [xiem-dashboard](../../xiem-dashboard) | Main React/Vite frontend dashboard |

---

### Layer 2 — KSA Country Core
Country-level services shared across all KSA verticals.

| Repository | Description | Key Integration |
|------------|-------------|-----------------|
| [compliance-engine-ksa](../../compliance-engine-ksa) | Compliance rules engine | SABER, SASO, ZATCA |
| [hs-customs-ksa](../../hs-customs-ksa) | HS code classification and tariffs | GCC Common External Tariff |
| [shipment-tracker-ksa](../../shipment-tracker-ksa) | Shipment tracking | FASAH Single Window |
| [procurement-ksa](../../procurement-ksa) | Purchase order management | — |
| [tax-engine-ksa](../../tax-engine-ksa) | VAT and customs duty calculation | ZATCA |
| [payments-ksa](../../payments-ksa) | Payment processing and e-invoicing | ZATCA FATOORA Phase 2 |
| [supplier-registry-ksa](../../supplier-registry-ksa) | Supplier registry and verification | Nitaqat |
| [municipality-ksa](../../municipality-ksa) | Municipality permit service | MOMRAH / Balady |
| [chamber-commerce-ksa](../../chamber-commerce-ksa) | Chamber of commerce certificates | SCCI |
| [dashboard-ksa](../../dashboard-ksa) | KSA reporting and analytics service | — |

---

### Layer 3 — KSA Construction Vertical
Construction-specific services built on top of the KSA country core.

| Repository | Description | Key Integration |
|------------|-------------|-----------------|
| [compliance-engine-ksa-construction](../../compliance-engine-ksa-construction) | Building codes and compliance | MOMRAH, Saudi Building Code |
| [hs-customs-ksa-construction](../../hs-customs-ksa-construction) | HS classification for building materials | Steel, cement, fixtures |
| [shipment-tracker-ksa-construction](../../shipment-tracker-ksa-construction) | Material shipment tracking | FASAH, Mawani |
| [procurement-ksa-construction](../../procurement-ksa-construction) | Contractor and materials procurement | — |
| [tax-engine-ksa-construction](../../tax-engine-ksa-construction) | VAT and duty for construction materials | ZATCA |
| [payments-ksa-construction](../../payments-ksa-construction) | Construction payment processing | ZATCA FATOORA |
| [supplier-registry-ksa-construction](../../supplier-registry-ksa-construction) | Contractor and supplier registry | Nitaqat |
| [municipality-ksa-construction](../../municipality-ksa-construction) | Building permits and approvals | MOMRAH / Balady |
| [chamber-commerce-ksa-construction](../../chamber-commerce-ksa-construction) | Contractor certification | SCCI |
| [dashboard-ksa-construction](../../dashboard-ksa-construction) | Construction compliance dashboard | — |

---

## Technology Stack

| Layer | Technology |
|-------|------------|
| Backend services | Node.js, TypeScript, Fastify |
| Frontend | React, Vite, Tailwind CSS |
| Database | PostgreSQL, Prisma ORM |
| Cache | Redis |
| Infrastructure | Docker, Docker Compose |
| API | REST, OpenAPI |
| Testing | Jest, 100% coverage on all services |

---

## GCC Rollout Plan

| Phase | Countries | Verticals | Status |
|-------|-----------|-----------|--------|
| Phase 1 | 🇸🇦 Saudi Arabia | Construction, Food & Beverage, Healthcare, Technology | Active |
| Phase 2 | 🇦🇪 UAE, 🇶🇦 Qatar | Manufacturing, Retail, Energy, Airlines, Automotive, Chemicals | Planned |
| Phase 3 | 🇰🇼 Kuwait, 🇧🇭 Bahrain, 🇴🇲 Oman | Textiles, Cosmetics, Agriculture | Planned |

---

## Key Compliance Systems

| System | Description |
|--------|-------------|
| ZATCA / FATOORA | Saudi e-invoicing and tax authority |
| SABER / SASO | Product certification and conformity |
| FASAH | Saudi customs single window |
| Nitaqat | Saudisation compliance verification |
| MOMRAH / Balady | Municipality and building permits |
| SCCI | Saudi Chamber of Commerce and Industry |
| Mawani | Saudi Ports Authority |
| PDPL | Saudi Personal Data Protection Law |

---

<div align="center">

**Synaptica Global** — Building the compliance infrastructure for GCC trade

*All repositories are private. Access restricted to authorized team members.*

</div>
