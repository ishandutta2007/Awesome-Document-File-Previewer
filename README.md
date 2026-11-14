# Awesome-Document-File-Previewer

## Top Document & File Previewer Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on Browser-Based Rendering, Multi-Format Viewing & Embedded SDKs*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Document & File Previewers**. These tools render PDFs, Office documents, images, and media directly in the browser—eliminating the need for users to download files or install native applications. The category spans embeddable commercial SDKs for product teams and self-hosted rendering engines for organizations seeking full control.

**Examples** include PSPDFKit (Nutrient), Accusoft PrizmDoc, Foxit PDF Web SDK, PDF.js, Apache PDFBox, and open-source alternatives like Open File Viewer and Papyrus (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted document rendering, open-source PDF engines, and community-driven file viewers—ideal for organizations seeking data sovereignty and avoiding per-document or per-seat SDK licensing. The open-source landscape is genuinely strong at the **rendering engine** layer (PDF.js, PDFBox, MuPDF) but thinner at the **turnkey viewer SDK** layer. **Open File Viewer** is the most ambitious unified viewer , **Papyrus** provides a modular PDF/EPUB SDK for React and React Native , and **docMentis udoc-viewer** offers WASM-based Office rendering without server round-trips .

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[PSPDFKit (Nutrient)](https://nutrient.io/)** | Enterprise document SDK for viewing, annotation, and editing across web, mobile, and desktop. Positioned as the premium commercial option for document-heavy products. | Quote-only (enterprise contract; historically five-figure annual minimums) | No free tier; trial via sales |
| **[Accusoft PrizmDoc](https://www.accusoft.com/)** | Document viewing and conversion SDK with server-side rendering. Supports PDF, Office, and CAD formats. | Quote-only (enterprise contract) | No free tier; demo via sales |
| **[Foxit PDF Web SDK](https://www.foxit.com/)** | Browser-based PDF viewer SDK from Foxit. Leverages Foxit's rendering engine for high-fidelity display and annotation. | Quote-only (per-application or per-user licensing) | Free trial available |
| **[Box View API](https://box.com/)** | Document conversion and viewing API that transforms files into HTML5 for browser display. | Quote-only (usage-based) | No free tier; demo via Box |
| **[Google Drive Viewer](https://drive.google.com/)** | Built-in viewer for files stored in Google Drive. Supports PDF, Office, images, and video without installation. | Free with Google account (15 GB shared storage) | **Free**: viewing for personal Google accounts |
| **[Microsoft Office Online Viewer](https://view.officeapps.live.com/)** | Free web-based viewer for Office documents via a simple URL parameter. No authentication required for public files. | **Free** | **Free**: public document viewing only |
| **[Filestack Document Viewer](https://www.filestack.com/)** | File handling platform with document preview capabilities as part of a broader upload/transform/deliver pipeline. | From **~$69/month** (Capterra listing) | Free tier available with limits |
| **[Cloudinary Document Viewer](https://cloudinary.com/)** | Media management platform with document preview as a secondary capability. **Credit-based pricing can become expensive if used primarily for storage** . | From **~$99/month** (Capterra listing) | Free tier available with limited transformations |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Open File Viewer](https://github.com/xushanpei/open-file-viewer)** | [![Stars](https://img.shields.io/github/stars/xushanpei/open-file-viewer?style=social&color=white)](https://github.com/xushanpei/open-file-viewer/stargazers) | **The most ambitious open-source unified file viewer.** MIT licensed, framework-agnostic (Vanilla JS, React, Vue, Svelte). Built-in plugins for **PDF, Office (DOCX/XLSX/PPTX), OFD, EPUB, XPS, images, media, archives, email, CAD, GIS, 3D, and text**. Client-side rendering—files stay in the browser and are not uploaded. Drop-in `<OpenFileViewer>` component with toolbar, themes, and multi-file queues, plus a plugin-first core for custom renderers . **Best for teams wanting a single viewer for all common attachment formats without commercial SDK licensing.** |
| **[Papyrus](https://github.com/solrachix/Papyrus)** | [![Stars](https://img.shields.io/github/stars/solrachix/Papyrus?style=social&color=white)](https://github.com/solrachix/Papyrus/stargazers) | **Modular open-source PDF/EPUB/TXT SDK for web and mobile.** Decoupled architecture: core state layer (Zustand), pluggable engines (**PDF.js on web, native on mobile**), and UI kits for React and React Native. Supports PDF, EPUB, TXT, CBZ, and CBR. Features event hooks for page/zoom/selection, background text search, themeable UI (light/dark/sepia/high-contrast), and Expo plugin for native builds . **Best for React/React Native teams needing a composable document SDK.** |
| **[docMentis udoc-viewer](https://github.com/docMentis/docmentis-udoc-viewer)** | [![Stars](https://img.shields.io/github/stars/docMentis/docmentis-udoc-viewer?style=social&color=white)](https://github.com/docMentis/docmentis-udoc-viewer/stargazers) | **WASM-powered universal viewer for PDF, DOCX, PPTX, and images.** Built from scratch with a **custom Rust/WebAssembly rendering engine—not PDF.js**. **Client-side only** (no server round-trips). Framework-agnostic (React, Vue, Angular, Svelte, plain HTML). MIT-licensed wrapper with free WASM engine. Features zoom/navigation, full-text search with highlighting, dark mode, and customizable UI . **Note: active development has moved to a new repository (docMentis udoc); this repo hosts v0.7.20.** Best for teams wanting high-fidelity Office rendering without server infrastructure. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[PDF.js](https://github.com/mozilla/pdf.js)** | [![Stars](https://img.shields.io/github/stars/mozilla/pdf.js?style=social&color=white)](https://github.com/mozilla/pdf.js/stargazers) | **Mozilla's PDF rendering engine—the foundation of most browser-based PDF viewing.** Renders PDF onto HTML5 Canvas. Supports annotations and AcroForms. **Apache 2.0 licensed.** Complex and worker-based, but battle-tested and used by Firefox, Papyrus, and countless other projects . **Best as a rendering engine to build upon, not a turnkey viewer.** |
| **[Apache PDFBox](https://github.com/apache/pdfbox)** | [![Stars](https://img.shields.io/github/stars/apache/pdfbox?style=social&color=white)](https://github.com/apache/pdfbox/stargazers) | **Comprehensive Java PDF library for rendering, text extraction, and form manipulation.** Apache 2.0 licensed. Development started in 2002. Renders to Gray/RGB/ARGB. **Java-only and complex API** . Best for Java server-side rendering or PDF manipulation workflows. |
| **[MuPDF](https://github.com/ArtifexSoftware/mupdf)** | [![Stars](https://img.shields.io/github/stars/ArtifexSoftware/mupdf?style=social&color=white)](https://github.com/ArtifexSoftware/mupdf/stargazers) | **Fast, comprehensive C rendering engine with WASM, Python, Java, and iOS/Android bindings.** Supports overprint, interactive features, and AcroForms. **AGPL v3 or commercial license from Artifex**—AGPL may be prohibitive for proprietary products . Best for performance-critical rendering where AGPL compliance is acceptable or commercial licensing is viable. |
| **[Peekin](https://github.com/sumanmichael/peekin)** | [![Stars](https://img.shields.io/github/stars/sumanmichael/peekin?style=social&color=white)](https://github.com/sumanmichael/peekin/stargazers) | **Lightweight read-only web file browser for local folders.** Python/MIT. Previews images (swipeable gallery), video, audio, PDF, rendered Markdown, and source code with syntax highlighting. **Runs fully offline** with password protection when shared on a network. HTML/SVG files are downloaded, never rendered (security). **Not an embeddable viewer**—a standalone folder-sharing tool . Best for local development or personal file browsing. |

**Frameworks for building custom systems**: Choose **Open File Viewer** for a unified drop-in viewer covering PDF, Office, media, and archives , **Papyrus** for a modular React/React Native SDK with PDF.js and native engines , or **docMentis udoc-viewer** for WASM-based Office rendering without server round-trips . For server-side PDF rendering in Java, **Apache PDFBox** provides the foundation. **None of these matches the annotation depth, forms support, or enterprise compliance certifications of PSPDFKit or PrizmDoc**—expect to build those layers yourself.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Document previewers render potentially sensitive files; **client-side rendering keeps files in the browser** (Open File Viewer, docMentis), while server-side rendering (PrizmDoc, PDFBox) requires secure transmission and temporary storage policies.
- **Licensing is the critical differentiator in open-source rendering.** **PDF.js and PDFBox are Apache 2.0**—permissive for commercial use . **MuPDF is AGPL v3**—proprietary products must either open-source their entire application or purchase a commercial license from Artifex . **Open File Viewer is MIT** , **Papyrus is open-source** (check repository license), and **docMentis udoc-viewer is MIT-licensed wrapper with a free WASM engine** . **Commercial platforms are quote-only**—PSPDFKit, PrizmDoc, and Foxit do not publish list pricing. **Filestack and Cloudinary are file platforms with preview as a secondary feature**, not purpose-built viewers—Cloudinary's credit system can become expensive if used primarily for storage rather than transformation . Validate licensing compatibility and rendering fidelity against your actual document corpus before committing.

---

**Made for developers, product teams, and organizations building document viewing infrastructure.**  
Let's make document and file previewing more open, embeddable, and cost-predictable.
