
# Ordering Service  The **Ordering Service** handles order creation, updates, and tracking.   It connects to the cart-service, payment-service, and inventory-service to ensure smooth ordering workflows.  ## Features - Create new orders - Update or cancel orders - Track order status 
# Analytics Service

The **Analytics Service** collects and processes event data from other services 
(e.g., ordering, payments, users, notifications) and provides aggregated reports 
and insights.

## Features
- Collect raw events from other services
- Query aggregated analytics
- Exposes REST API with Swagger auto-doc
- Extensible for plugging in a data warehouse (e.g., BigQuery, Snowflake, PostgreSQL)

## Tech Stack
- Python 3.11
- FastAPI
- SQLite (dev) / PostgreSQL (prod)
- Docker + Docker Compose

## Running Locally
```bash
docker-compose up --build
