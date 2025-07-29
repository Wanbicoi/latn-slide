---
title: Authentication & Security
layout: center
---

# Nginx Authentication Sequence

```mermaid
sequenceDiagram
  participant User
  participant Nginx as "Nginx Reverse Proxy"
  participant Auth as "Supabase Auth"
  participant App as "Upstream App<br/>(React/OHIF)"

  Note over Nginx: "All requests pass through Nginx first."

  User->>Nginx: "GET /protected-resource (with auth cookie)"
  Nginx->>Auth: "auth_request subrequest to /auth/v1/user"
  Auth-->>Nginx: "200 OK (JWT is valid)"
  Nginx->>App: "Proxy original request"
  App-->>Nginx: "200 OK (Response with resource)"
  Nginx-->>User: "Response with resource"

  alt "Invalid/Missing Token"
    User->>Nginx: "GET /protected-resource (no/bad cookie)"
    Nginx->>Auth: "auth_request subrequest"
    Auth-->>Nginx: "401 Unauthorized"
    Nginx-->>User: "Redirect to /login page"
  end
```

---
layout: two-cols
---

# Security Implementation

::left::

## 🔐 **Centralized Authentication**
- Single source of truth for auth state
- Nginx reverse proxy handles all requests
- Supabase JWT validation
- Automatic session management

## 🛡️ **Protection Mechanisms**
- All routes protected by default
- Cookie-based authentication
- Automatic token validation
- Secure redirection on failure

::right::

## 🌐 **Micro-Frontend Integration**
- Unified auth across React app & OHIF
- Seamless user experience
- No auth state duplication
- Cross-component session sharing

## ⚡ **Performance Benefits**
- Auth validation at proxy level
- Reduced backend auth load
- Cached authentication decisions
- Efficient request routing