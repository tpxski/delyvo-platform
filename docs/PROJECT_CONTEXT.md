# DELYVO Project Context

## Identity
- Brand: DELYVO
- Descriptor: Delivery & Logistics
- Primary market: Algeria
- Initial model: independent motorcycle delivery service
- Long-term model: multi-driver logistics platform

## Services
- DELYVO Dental
- DELYVO Express / General
- E-commerce delivery
- Restaurant delivery
- Personal delivery

Dental is a specialization, not a separate company.

## Customer types
- Dental professional
- Dental laboratory
- E-commerce business
- Restaurant / food business
- Personal customer

Customer accounts are required/preferred for the MVP.

## Delivery workflow
Created -> Accepted -> To Collect -> Collected -> In Transit -> Arrived -> Delivered

Exceptions: Cancelled, Returned, Problem / Exception

Example tracking ID: DLV-2026-00482

## Dental specialization
The founder has dental CAD/CAM experience. Dental deliveries may include alginate impressions, silicone/elastomer impressions, bite registrations, dental models, crowns, bridges, implant-related work, provisional work and consumables.

Use a case reference instead of unnecessary patient-identifying information.

## Admin control
The founder requires a SUPER ADMIN control center with control over customers, drivers, deliveries, pricing, zones, services, workflows, permissions, notifications, reports and activity logs.

## Customer dashboard
Customers need account, profile, new delivery, active deliveries, history, tracking and statistics. Forms adapt to customer type.

## Driver
The initial system may have one driver, but the architecture must support multiple drivers later.

## Architecture decision
Fleetbase is the initial logistics foundation. DELYVO is the product layer: brand, customer experience, service-specific workflows and business logic.

Do not make the DELYVO experience dependent on Fleetbase's default UI.

## Cost strategy
Development should remain zero-cost where practical: local development, self-hosted open-source software, GitHub and AI coding tools. Domain and paid hosting come later.

## Current stage
Foundation / Architecture.

Completed:
- Brand selected
- Services defined
- Customer types defined
- Admin requirements defined
- Fleetbase selected as initial foundation
- GitHub repository created
- Permanent documentation established

Next:
1. Audit Fleetbase architecture and license constraints.
2. Define integration boundaries.
3. Define domain/data model.
4. Install Fleetbase locally.
5. Build DELYVO MVP.
