---
title: System Architecture
# layout: right
---

<!-- # System Architecture Overview -->

<img src="../images/architecture.svg" alt="Architecture" style="max-height: 500px; width: auto; margin: 0 auto; display: block; background: white; padding: 20px; border-radius: 8px; box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);" />

---

# Architecture Benefits

## 🔒 **Security & Authentication**
- Centralized authentication via Nginx reverse proxy
- Unified access control across micro-frontends
- Secure DICOM data handling

## ⚡ **Performance & Scalability**
- Declarative caching with TanStack Query
- Automated cache invalidation
- Asynchronous workflow orchestration

## 🔧 **Integration & Flexibility**
- Multi-layered abstraction with PostgreSQL views
- Database-centric automation engine
- Open-source platform integration