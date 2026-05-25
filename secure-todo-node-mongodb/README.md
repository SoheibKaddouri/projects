## Secure To-Do List Application

A secure, full-stack Task Management platform engineered to showcase server-side routing architecture, session-based state isolation, and persistent relational data storage. The application delivers robust user sandboxing and complete CRUD data pipelines using a compiled backend architecture.

### 🛠️ Tech Stack & Focus Areas
* **Backend Environment:** Node.js / Express.js Framework
* **Persistent Storage:** MongoDB / Mongoose ODM (Object Data Modeling)
* **View Engine:** Compiled Server-Side Embedded JavaScript (EJS) Templates
* **Security & Cryptography:** Stateful Session Management (`express-session`), Cryptographic Hashing (`bcrypt`)

### 📈 Core Business Value & Engineering Impact
* **Cryptographic Credential Protection:** Implements an asynchronous blowfish-backed key-derivation hashing pipeline using 10 salt rounds to obfuscate user credentials, ensuring zero plain-text passwords hit the persistence layer.
* **Stateful User Isolation (Sandboxing):** Leverages signed, server-side session cookies to isolate client execution states. Users are strictly sandboxed, preventing unauthorized cross-tenant data access and securing core operational routes.
* **Schema-Level Data Sanitation:** Utilizes strict Mongoose ODM validation parameters (including string trimming and explicit uniqueness indexing) to enforce data integrity and eliminate malicious space-injection overhead.

### 📁 Platform Architecture Breakdown
The application structure isolates backend server routines from model definitions:
* **Central Application Router (`index.js`):** Coordinates core system orchestration, mounting express middleware, establishing the asynchronous MongoDB database handshake, and exposing authenticated REST endpoints.
* **Relational Persistence Models (`/models`):** Specialized database layer definitions including `TodoUser` schemas for account tracking and `TodoTask` schemas utilizing schema-level object relations (`ref`) to associate records to specific users.
* **Server-Rendered Templates (`/views`):** Lightweight UI files compiled dynamically on the server to expose customized user data views exclusively to valid, active session holders.

### 🌐 Live Interactive Demo
To see the application execution pipelines, schema setups, and full backend configuration files within an isolated codebase environment, check out the dedicated project repository here: [Secure To-Do List Code Repository](https://github.com/soheibkaddouri/secure-todo-node-mongodb)
