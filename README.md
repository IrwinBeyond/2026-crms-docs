# CRMS Documentation

Comprehensive documentation repository for the
**Classroom / Room Management System (CRMS)**.

---

## Project Title

CRMS — Classroom / Room Management System Documentation

---

## Description

This repository contains the official documentation for the CRMS full-stack system.

CRMS is a room borrowing management platform designed to demonstrate structured domain enforcement, lifecycle control, query abstraction, and dashboard aggregation.

This documentation repository centralizes:

* System overview
* Architecture explanation
* API contract reference
* Release documentation
* Setup guides
* Version alignment
* Development workflow standards

It exists to ensure clarity, reproducibility, and maintainability of the CRMS project.

---

## Features

* Full-stack architecture documentation
* Backend API contract reference
* Frontend module overview
* Status transition model documentation
* Query contract explanation
* Versioning strategy documentation
* Release governance documentation
* Development workflow guidelines

---

## System Components

CRMS consists of:

* **Frontend Repository**

  * React + TypeScript
  * Query engine
  * Archive mode
  * Dashboard UI

* **Backend Repository**

  * ASP.NET Core
  * Entity Framework Core
  * MySQL
  * Status transition enforcement
  * Conflict detection
  * Dashboard aggregation

---

## Architecture Overview

CRMS follows a layered and modular structure:

### Backend

Controller → Service → Data → Database

* Domain logic enforced at service layer
* Soft delete globally filtered
* Enum-based status modeling
* Strict state transition control

### Frontend

Feature-based modular structure:

* Borrowing module
* History module
* Dashboard module
* Reusable UI component system

---

## Tech Stack

### Backend

* ASP.NET Core
* Entity Framework Core
* MySQL
* Swagger

### Frontend

* React
* TypeScript
* Vite
* Axios
* TailwindCSS
* Lucide React

---

## Usage

This repository serves as a reference.

Typical usage includes:

* Reviewing architecture before contributing
* Verifying API contract alignment
* Understanding release structure
* Reviewing versioning policy
* Studying system design decisions

---

## Environment Variables

This documentation repository does not require environment variables.

For system operation, refer to:

### Frontend `.env`

```
VITE_API_URL=http://localhost:5233/api
```

### Backend `appsettings.json`

```
ConnectionStrings:DefaultConnection
Cors:AllowedOrigins
```

---

## Development Workflow

Branching strategy:

```
main        → Stable release
develop     → Active development
feature/*   → Feature implementation
fix/*       → Bug fixes
```

Tagging is performed on `main`.

Semantic Versioning:

* PATCH → Bug fixes
* MINOR → Backward-compatible feature addition
* MAJOR → Breaking changes

---

## Version Alignment

Stable Release:

* Frontend: v1.0.0
* Backend: v1.0.0

Future releases must maintain API contract compatibility unless major version changes.

---

## Contributing

Contributions should:

* Follow established branching strategy
* Maintain API contract stability
* Include changelog updates
* Avoid breaking changes without version increment

Pull requests should clearly describe:

* Scope
* Impact
* Compatibility considerations

---

## License

This project is developed for academic and portfolio demonstration purposes.

You may reuse the structure and ideas for learning or educational use.
[MIT License](LICENSE)

---

## Author

Developed as a structured full-stack academic project demonstrating:

* Domain-driven enforcement
* Query abstraction
* Lifecycle state management
* Release engineering discipline

---

## Future Roadmap

Planned improvements:

* Role-Based Access Control (RBAC)
* Authentication integration
* Audit logging
* Production deployment configuration
* Docker containerization
* CI/CD pipeline