# Rental Management WebGIS System

A WebGIS platform for rental property and apartment building management, integrating spatial topology data with property administration.

---

## Project Overview
This project provides an end-to-end solution for landlords, property managers, and tenants:
* **Interactive 2.5D Building Viewer**: Visualize floor-by-floor layouts and apartment occupancy using custom topological GIS models.
* **Property & Asset Management**: Centralized management of buildings, floors, rooms, and facilities.
* **Operational Workflows**: Manage rental contracts, service indices (electricity, water), automated billing, and tenant issues.
* **Tenant Portal**: Self-service portal for tenants to view billing details and contract statuses.

---

## Technology Stack
* **Backend**: FastAPI, SQLAlchemy, Alembic, PostgreSQL
* **Frontend**: Jinja2 Templates, HTML5/CSS3, JavaScript (ES6), Leaflet.js
* **Spatial Engine**: Relational Topological Data Structure (Point - Node - Arc - Polygon)

---

## Project Structure
```text
webgis-workspace/
├── app/                  # Application source code
│   ├── core/             # Configuration, security & constants
│   ├── crud/             # Database queries & business logic
│   ├── routers/          # API endpoints & view controllers
│   ├── static/           # Static assets (CSS, JS, media storage)
│   └── templates/        # Jinja2 presentation templates
├── data/                 # System fixtures, demo datasets & GeoJSON samples
├── scripts/              # CLI scripts for database init & data seeding
├── .env.example          # Environment variables template
├── requirements.txt      # Project dependencies
└── README.md             # Project documentation
```

---

## Getting Started

### 1. Prerequisites
* Python 3.10+
* PostgreSQL 14+

### 2. Environment Setup
```bash
# Create and activate virtual environment
python -m venv .venv
.venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Configure environment variables
copy .env.example .env
```

---

## Development Status
- [x] Project scaffolding & repository initialization
- [ ] Database setup & schema migration (In Progress)
- [ ] Core authentication & authorization
- [ ] 2.5D Spatial topology engine
- [ ] Administrative modules & Tenant portal