# alvisio – Technical Documentation & Architecture Overview

This repository provides a high‑level, non‑sensitive technical overview of **alvisio**, a lightweight and long‑term stable content management system designed for multi‑domain environments, professional customer projects and efficient content workflows.

alvisio operates multiple independent websites from a shared codebase while keeping all customer data strictly isolated through separate databases and domain‑specific configuration.

This documentation focuses on architectural concepts, design principles and the philosophy behind alvisio — without exposing internal implementation details.

---

## 1. Core Architecture Principles

alvisio is built on a set of durable architectural principles:

- **Shared Codebase**  
  One installation powers multiple independent websites.

- **Strict Data Isolation**  
  Each domain uses its own database and configuration.

- **Minimal Dependencies**  
  No plugin ecosystem, no external frameworks, no third‑party modules.

- **Separation of Concerns**  
  Content, layout, logic and configuration are cleanly separated.

- **Performance Through Simplicity**  
  Efficient SQL usage, lightweight rendering, predictable behavior.

- **Security Through Controlled Architecture**  
  No external code paths, no plugin attack surface, isolated tenants.

---

## 2. Automated CMS – What makes alvisio different

alvisio is not a traditional content management system.  
It is an **automated CMS (aCMS)**: a system that applies professional design and layout techniques automatically, without requiring editors to have any design knowledge.

### Target Audience

alvisio is designed for organizations where website content is created by people without formal design training.  
Unlike traditional CMS platforms that rely on manual layout decisions, alvisio automates design, typography and image processing.  
This makes it ideal for companies where editors want to publish content quickly without dealing with layout tools, color choices or formatting rules.

### Automated Design & Layout Techniques

alvisio analyses content, images, structure and context to generate visually consistent, high‑quality layouts.  
This includes automated techniques such as:

- **Responsive image processing**  
  Images are automatically downscaled into multiple resolutions for optimal loading performance.

- **Automatic color extraction**  
  Dominant and accent colors are identified and used for frames, text boxes, titles and other design elements.

- **Motif protection**  
  Important areas of an image are preserved across different aspect ratios to avoid unwanted cropping.

- **Typographic optimization**  
  Headings are automatically balanced across multiple lines for harmonious visual appearance.

- **Semantic punctuation handling**  
  Hyphens are converted into proper en‑ or em‑dashes when used as thought dashes.

- **Non‑breaking units**  
  Units such as “mm”, “km”, “kg”, “°C” remain attached to their numbers (e.g. “3 mm”).

These are only a few examples on the editor‑facing side.  
Internally, alvisio applies many more automated processes to ensure consistent quality, stability and performance across all domains.

### Further Reading

- [Target Audience](automated-cms/target-audience.md)  
- [Automated CMS Overview](automated-cms/overview.md)

---

## 3. Multi‑Tenant Concept

alvisio supports multi‑domain setups through:

- domain‑based configuration loading  
- database routing per tenant  
- isolated content and media  
- shared updates across all domains  
- consistent behavior across customer installations  

This allows dozens of websites to run on one codebase while remaining fully independent.

---

## 4. Content Management

alvisio provides a structured and efficient content workflow:

- page and story management  
- category systems  
- integrated media handling  
- editor‑based content creation  
- optional versioning and revision workflows  
- customizable navigation structures  

The system is designed for clarity and long‑term maintainability.

---

## 5. Template & Layout System

alvisio separates content from presentation:

- flexible template structure  
- reusable layout components  
- mobile‑friendly rendering  
- domain‑specific design configuration  
- clean separation between HTML, logic and content  

This allows each website to have its own visual identity while sharing the same underlying engine.

---

## 6. Extensibility

alvisio is modular by design:

- configurable feature sets  
- domain‑specific extensions  
- optional custom modules  
- clean integration points without exposing internal APIs  

The system grows with customer needs while maintaining architectural integrity.

---

## 7. Security Philosophy

alvisio follows a conservative, controlled security model:

- no third‑party plugins  
- no external dependencies  
- isolated databases per domain  
- server‑side validation  
- predictable request handling  
- minimal attack surface  

This avoids common CMS vulnerabilities caused by plugin ecosystems or shared data structures.

---

## 8. Performance Philosophy

alvisio is optimized for long‑term efficiency:

- minimal SQL queries per request  
- lightweight rendering pipeline  
- caching‑friendly output  
- no heavy frameworks  
- predictable performance across all domains  

The system is designed to remain fast even after many years of operation.

---

## 9. Typical Use Cases

alvisio is used in:

- corporate websites  
- educational platforms  
- customer‑specific portals  
- multi‑domain environments  
- long‑term maintained web projects  

Its architecture makes it suitable for stable, professional deployments.

---

## 10. License

This documentation is provided for informational purposes.  
alvisio itself is proprietary software and not publicly distributed.
