# homteq Smart Home E-Commerce Platform

A dynamic, full-stack e-commerce web application engineered for the homteq smart home ecosystem. The platform hosts an interactive customer-facing product catalog, a persistent session-driven shopping basket, secure authentication layers, and an integrated order fulfillment management portal.

## 🛠️ Tech Stack & Focus Areas
* **Backend Core:** Functional PHP 8.x / State Management & Session Handling / Relational MySQL
* **Database Management:** Relational Schema Architecture / Referential Integrity / Automated Seeding
* **Design Methodology:** Tabular Layout Optimization, Data-Driven UI Forms, Clean Data Stream Encoding

## 📈 Core Business Value & Engineering Impact
* **Unified Commerce Flow:** Demonstrates how a single server-side application can securely manage complex user states, transitioning customers smoothly from guest browsing to active session-based cart building and checkout processing.
* **Relational Database Integrity:** Engineered with cascading relational foreign keys to completely eliminate orphan records across inventory records, dynamic checkouts, and customer databases.
* **Data Stream Stabilization:** Resolved critical encoding mismatches by mapping data streams to standard HTML entities (`&pound;`), ensuring currency presentation remains cross-browser compliant.

## 📁 Platform Architecture Breakdown
The project is architected into specific user flows:
1. **Interactive Catalog:** A data-driven product showcase pulling live inventory records from the database, equipped with dynamic quantity selection nodes.
2. **Persistent Shopping Basket:** A session-validated tracking engine allowing real-time cart additions, selective item removals, and automatic subtotal math calculations.
3. **Secure Authentication Gateways:** Tiered security vectors separating permissions, navigational headers, and functional states between standard Customers and system Administrators.
4. **Administrative Fulfillment Center:** A backend order desk allowing platform staff to process pending customer transactions, analyze totals, and track delivery states.

## 🌐 Live Interactive Demo
* To see the platform code structure and backend database schemas in real-time within an interactive repository environment, check out the project codebase here: **[homteq Smart Home Code Repository](https://github.com/SoheibKaddouri/homteq-ecommerce-platform)**
