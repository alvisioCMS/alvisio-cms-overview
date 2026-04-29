# alvisio – Technical Documentation & Architecture Overview

This repository provides a high‑level, non‑sensitive technical overview of **alvisio**,  
a lightweight and long‑term stable content management system designed for:

- multi‑domain environments  
- professional customer projects  
- efficient, zero‑training editorial workflows  

alvisio operates multiple independent websites from a shared codebase while keeping all customer data strictly isolated through separate databases and domain‑specific configuration.

This documentation focuses on architectural concepts, design principles and the philosophy behind alvisio — without exposing internal implementation details.

---

## Core Architecture Principles

alvisio is built on durable architectural principles:

- **Shared Codebase** — one installation powers multiple independent websites.  
- **Strict Data Isolation** — each domain uses its own database and configuration.  
- **Minimal Dependencies** — no plugin ecosystem, no external frameworks.  
- **Separation of Concerns** — content, layout, logic and configuration are cleanly separated.  
- **Performance Through Simplicity** — efficient SQL usage, lightweight rendering.  
- **Security Through Controlled Architecture** — no external code paths, no plugin attack surface.

Further reading:  
- [Architecture Overview](architecture/overview.md)  
- [Multi‑Tenant Concept](architecture/multi-tenant.md)  
- [Philosophy](architecture/philosophy/README.md)

---

## Automated CMS – Key Concepts

alvisio is not a traditional CMS.  
It is an **Automated CMS (aCMS)**:  
a system that applies professional design and layout techniques automatically, without requiring editors to have design knowledge.

### Automated Design Interpretation
alvisio interprets the design system and applies it consistently across all content.  
→ [Automated Design](features/automated-design.md)

### Automated Media Optimization
Images are processed, optimized and delivered intelligently.  
→ [Automated Media Optimization](features/automated-media-optimization.md)

### Automated Editorial Workflows
Zero‑training editing, automatic formatting, error prevention.  
→ [Automated Editorial Workflows](features/automated-editorial-workflows.md)

### Automated SEO & Metadata
Automatic generation of meta tags, OpenGraph, Twitter Cards, JSON‑LD.  
→ [Automated SEO & Metadata](features/automated-seo-metadata.md)

Further reading:  
- [Automated CMS Overview](automated-cms/overview.md)  
- [Target Audience](automated-cms/target-audience.md)

---

## Campaign Tracking (Cookie‑free)

alvisio includes a built‑in campaign tracking mechanism. Each campaign receives a unique ID and every request is logged server‑side  
without using cookies, JavaScript or external analytics tools.

This enables tracking of:

- links on external websites  
- QR codes (business cards, vehicles, posters, flyers)  
- email signatures  
- offline and online marketing materials  

Because no personal data is stored and no cookies are used, this mechanism is fully  
GDPR‑compliant and works even in environments where traditional analytics are blocked.

---

## Multi‑Tenant Concept

alvisio supports multi‑domain setups through:

- domain‑based configuration loading  
- database routing per tenant  
- isolated content and media  
- shared updates across all domains  

This allows dozens of websites to run on one codebase while remaining fully independent.

→ See: [Multi‑Tenant Architecture](architecture/multi-tenant.md)

---

## Content Management

alvisio provides a structured and efficient content workflow:

- page and story management  
- category systems  
- integrated media handling  
- editor‑based content creation  
- optional versioning  
- customizable navigation structures  

The system is designed for clarity and long‑term maintainability.

---

## Template & Layout System

alvisio separates content from presentation:

- flexible template structure  
- reusable layout components  
- mobile‑friendly rendering  
- domain‑specific design configuration  

Each website can have its own visual identity while sharing the same engine.

---

## Extensibility

alvisio is modular by design:

- configurable feature sets  
- domain‑specific extensions  
- optional custom modules  
- clean integration points without exposing internal APIs  

The system grows with customer needs while maintaining architectural integrity.

---

## Security Philosophy

alvisio follows a conservative, controlled security model:

- no third‑party plugins  
- no external dependencies  
- isolated databases per domain  
- server‑side validation  
- predictable request handling  

This avoids common CMS vulnerabilities caused by plugin ecosystems.

---

## Performance Philosophy

alvisio is optimized for long‑term efficiency:

- minimal SQL queries per request  
- lightweight rendering pipeline  
- caching‑friendly output  
- no heavy frameworks  

The system remains fast even after many years of operation.

---

## Typical Use Cases

alvisio is used in:

- corporate websites  
- educational platforms  
- customer‑specific portals  
- multi‑domain environments  
- long‑term maintained web projects  

Its architecture makes it suitable for stable, professional deployments.

---

## License

This documentation is provided for informational purposes.  
alvisio itself is proprietary software and not publicly distributed.

---

## About alvisio

alvisio has been continuously developed **since 2001** by **Ulrich Albrecht**  
(Albrecht: Agentur für Unternehmensdarstellung, Bochum, Germany).

The system originated as a custom CMS for professional corporate communication  
and has evolved into a fully automated content management system (aCMS)  
focused on design consistency, performance, and zero‑training editorial workflows.

### Contact

Albrecht: Agentur für Unternehmensdarstellung  
Thorner Str. 21  
D - 44789 Bochum  
Germany  

[Contact Form (secure)](https://www.agenturalbrecht.de/m.php?get=Feedback)  
[https://agenturalbrecht.de](https://www.agenturalbrecht.de/index.php?ca=16)
