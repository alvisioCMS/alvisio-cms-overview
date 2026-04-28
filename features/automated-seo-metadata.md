
# Automated SEO & Metadata

alvisio automatically generates all essential SEO metadata for every page — without requiring editors to understand search engine optimization, structured data, or HTML.  
This ensures consistent, technically correct SEO output across the entire website.

Traditional CMS systems rely on plugins, manual configuration, or editor knowledge.  
alvisio integrates SEO logic directly into the system and adapts it to each page type.

---

## Key Capabilities

### 1. Automatic Meta Titles and Descriptions
alvisio generates:

- `<title>`  
- `<meta name="description">`  
- `<meta name="publisher">`  
- `<meta name="robots">`  

based on the content and structure of each page.

Editors do not need to write or maintain SEO metadata manually.

---

### 2. Automatic Canonical URLs
alvisio generates a correct `<link rel="canonical">` tag for every page to prevent duplicate content issues.

---

### 3. Automatic Social Media Metadata (Twitter & OpenGraph)
alvisio automatically inserts:

- `twitter:title`  
- `twitter:description`  
- `twitter:url`  
- `twitter:site`  
- `twitter:creator`  

Images are selected based on the page’s main visual content.

OpenGraph metadata is generated where appropriate.

---

### 4. Automatic RSS Feed Linking
alvisio inserts:
<link rel="alternate" type="application/rss+xml" ... >

when a page or section supports RSS feeds.

---

### 5. Automatic Technical Metadata
alvisio generates:

- `<meta name="generator">`  
- `<meta name="format-detection" content="telephone=no">`  
- `<meta http-equiv="cache-control">`  
- `<meta http-equiv="pragma">`  
- `<meta name="copyright">`  

ensuring consistent technical SEO and browser behavior.

---

### 6. Automatic JSON‑LD Structured Data
alvisio inserts JSON‑LD blocks tailored to the specific page type.  
Examples include:

#### **Organization**
```json
{
    "@context": "https://schema.org",
    "@type": "Organization",
    "name": "...",
    "url": "...",
    "logo": "...",
    "description": "...",
    "email": "...",
    "foundingDate": "...",
    "founder": "...",
    "image": "...",
    "address": { ... },
    "telephone": "...",
    "sameAs": [ ... ]
}
```
#### **Produkt**
```json
{
    "@context": "https://schema.org",
    "@type": "Product",
    "name": "alvisio",
    "url": "...",
    "description": "...",
    "image": "...",
    "brand": { ... },
    "offers": { ... }
}
```
#### **WebPage**
```json
{
    "@context": "https://schema.org",
    "@type": "WebPage",
    "name": "...",
    "url": "...",
    "description": "...",
    "breadcrumb": { ... },
    "mainEntity": [ ... ]
}
```
These blocks are generated automatically based on:

- **page type**
- **page content**
- **design configuration**
- **site‑wide settings**

Editors do not need to understand JSON‑LD or schema.org.

---

## 7. Automatic Image Metadata

alvisio generates:

- alt texts (when possible)
- image dimensions
- optimized filenames
- WebP versions

This improves SEO, accessibility, and performance simultaneously.

---

## Why This Is Unique

Traditional CMS systems (WordPress, Typo3, CraftCMS):

- require plugins for SEO
- rely on editors to fill out metadata
- do not generate JSON‑LD automatically
- often produce inconsistent or missing metadata
- depend on manual configuration

alvisio provides:

- fully automated SEO metadata
- automatic JSON‑LD generation
- consistent OpenGraph and social metadata
- automatic canonical URLs
- zero training for editors
- SEO‑correct output on every page

This is a core component of alvisio’s identity as an **Automated CMS**.
