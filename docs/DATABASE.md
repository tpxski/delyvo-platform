# DELYVO Data Model

Initial domain model only; this is not yet the final database schema.

Core entities:
- User: id, role, name, email, phone, status, created_at
- Customer Profile: user, customer type, business data, contacts, addresses
- Delivery: tracking ID, customer, service, pickup, destination, driver, status, priority, price, notes, timestamps
- Dental Delivery: case reference, material/work type, urgency, handling instructions
- Driver: user, status, vehicle, location, availability
- Payment: delivery, amount, method, status
- Proof of Delivery: delivery, proof type, timestamp

First map these concepts to existing Fleetbase entities and APIs. Avoid duplicate custom tables when Fleetbase already provides the required entity.
