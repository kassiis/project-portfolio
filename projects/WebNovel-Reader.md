# Web Novel Studio & Reader

**GitHub Repository:** `kassiis/webnovel-reader`  
**Source code:** Private repository  
**Project Category:** Web Applications & Media Platforms  
**Development Status:** Active / Fully Functional Web App  

---

## 1. Overview

**Web Novel Studio & Reader** is a responsive digital reading environment and authoring suite designed for serial literature and web novels. The application features customizable reading typography, chapter management tools, and a decoupled data abstraction layer supporting both client-side storage and external database connectivity.

---

## 2. Project Purpose

Serial fiction readers and independent authors require streamlined, distraction-free digital interfaces that work seamlessly across desktop and mobile screens without heavyweight framework dependencies. This project provides:

- An ergonomic, book-like reading interface with real-time reading customization.
- An intuitive writing studio allowing authors to draft, organize, and paginate chapters with instant word count analytics.
- A decoupled data layer that operates out-of-the-box locally while providing structured adapter interfaces for cloud backends.

---

## 3. Key Capabilities

- **Reader Experience:**
  - Responsive layout optimized for long-form reading across mobile, tablet, and desktop viewports.
  - Reader preferences including font sizing, line spacing, margins, and dark/light color themes.
  - Chapter navigation controls, reading progress retention, and novel metadata cards.
- **Authoring Studio:**
  - Novel creation workflow supporting title, author, genre classification, synopsis, and cover art.
  - Chapter editor with automatic word count analysis and chronological sorting.
  - Interactive chapter management (adding, updating, and removing chapters).
- **Decoupled Data Architecture:**
  - Architectural separation between user interface components and persistence logic (`NovelDataService`).
  - Seamless fallback to browser local storage for offline operation.
  - Clean adapter hooks designed for plug-and-play integration with remote REST APIs, PostgreSQL/MySQL databases, or Backend-as-a-Service (BaaS) platforms.
- **Lightweight Development Server:** Bundled Python HTTP server facilitating instant local preview and testing with zero external package installation.

---

## 4. Technologies Used

- **Frontend Core:** HTML5 Semantic Markup, Modern CSS3 (CSS Grid, Flexbox, Custom Properties)
- **Client Scripting:** JavaScript (ES6+, Object-Oriented Architecture, Async/Await)
- **Persistence Layer:** Browser LocalStorage API with extensible REST/SQL/BaaS adapter patterns
- **Local Tooling:** Python 3 standard library (`http.server`)

---

[← Return to Project Portfolio](../README.md)
