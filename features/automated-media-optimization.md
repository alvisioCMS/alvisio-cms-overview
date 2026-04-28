
# Automated Media Optimization

alvisio handles the entire image and media processing pipeline automatically.  
Editors upload a file once — alvisio takes care of everything else: scaling, compression, format conversion, cropping, naming, and performance‑optimized delivery.

Unlike traditional CMS systems that rely on plugins or manual configuration, alvisio provides a fully integrated, intelligent media pipeline that adapts to the design system and the visitor’s device capabilities.

---

## Key Capabilities

### 1. Automatic Scaling into Multiple Sizes
When an image is uploaded, alvisio automatically generates several optimized versions in different resolutions.  
These versions are stored in dedicated “thumbs” folders and used depending on:

- layout size  
- device resolution  
- network speed  
- performance requirements  

Editors never have to think about image sizes or responsive behavior.

---

### 2. Automatic Compression
alvisio automatically compresses images to an optimal balance of:

- visual quality  
- file size  
- loading speed  

This ensures consistently fast performance without requiring editors to understand image formats or compression settings.

---

### 3. Automatic WebP Generation
Every uploaded image is automatically converted into WebP versions.  
This provides:

- significantly smaller file sizes  
- faster loading  
- modern browser compatibility  

alvisio chooses the best format automatically during rendering.

---

### 4. Automatic or Manual Cropping (including rotation)
Editors can rotate or crop images manually in the admin interface.  
alvisio always performs these operations on the **original file**, ensuring:

- no quality loss  
- reversible edits  
- future‑proof transformations  

The original file is never overwritten.

---

### 5. Intelligent Delivery Based on Layout, Device, and Network
When rendering a page, alvisio selects the optimal image version based on:

- the actual layout size of the image frame  
- the visitor’s screen resolution  
- the visitor’s current network speed  

This goes far beyond HTML5 `srcset`, because alvisio also evaluates the **layout context**:

- If the layout uses a small image frame (e.g., overview pages), alvisio delivers a small image — even on a high‑resolution display.  
- If the visitor has a high‑resolution display but a slow connection, alvisio prioritizes loading speed and delivers a lower‑resolution version.  
- If the visitor has both high resolution and fast connection, alvisio delivers a high‑quality version.

This ensures optimal performance and visual quality for every visitor.

---

### 6. Automatic Filename Repair and Editor‑Friendly Naming
When uploading files like IMG12345678.JPG, editors can rename them to meaningful titles such as:
Messestand (2026)
alvisio automatically converts this into a web‑safe filename:
Messestand_2026.jpg
and generates all required WebP versions:
Messestand_2026.webp


Editors always work with a single logical file, while alvisio manages all technical variants in the background.

---

## Why This Is Unique

Traditional CMS systems (WordPress, Typo3, CraftCMS):

- rely on plugins for image processing  
- do not consider layout size when selecting image resolutions  
- do not adapt to network speed  
- do not maintain a clean original file for reversible edits  
- do not repair filenames automatically  
- require editors to understand responsive image handling  

alvisio provides:

- a fully integrated media pipeline  
- intelligent, context‑aware image delivery  
- automatic optimization without configuration  
- consistent performance across all devices  
- zero training for editors  

This is a core component of alvisio’s identity as an **Automated CMS**.

