# DELYVO Architecture

## Principle
DELYVO is a product built around an open-source logistics foundation.

Conceptual flow:
DELYVO UI -> DELYVO business layer -> Fleetbase capabilities -> PostgreSQL / Redis / storage / realtime services

## Layers
- Presentation: public website, customer portal, owner/admin dashboard, driver interface.
- Application: authentication, customers, deliveries, pricing, service workflows, notifications, permissions and reporting.
- Logistics foundation: Fleetbase orders, dispatch, drivers, tracking, locations, proof of delivery, workflows and APIs where appropriate.
- Data: PostgreSQL, Redis and required storage.

## Ownership boundary
Prefer configuration, extensions and integration layers before modifying Fleetbase core.

Any core modification must document file, reason, impact, upgrade implications and license implications.

## Environments
- Development: local machine, Docker where appropriate.
- Testing: local/staging before public release.
- Production: decide later based on cost, PostgreSQL, Redis, workers, storage, realtime and backups.

## Security
Never commit secrets, API keys, database passwords, authentication secrets, production credentials or real customer/patient data.
Use environment variables and .env.example files.

## Scalability
Support future multiple drivers, admins, customer organizations, cities and mobile apps.

## Important
Verify the exact Fleetbase version and source before relying on APIs or internals.
