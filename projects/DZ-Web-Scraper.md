# Algerian Web Scraper & Crawler

**GitHub Repository:** `kassiis/dz-web-scraper`  
**Source code:** Private repository  
**Project Category:** Automation & Web Scraping  
**Development Status:** Active / Production-Ready Utility  

---

## 1. Overview

**Algerian Web Scraper & Crawler** is a high-performance Python data extraction engine and crawler specialized in extracting structured data from web targets, with specialized capabilities for analyzing Algerian web infrastructure, regional contact indicators, and administrative identifiers.

---

## 2. Project Purpose

Extracting clean, structured data from dynamic websites often requires custom handling for localized regional formats and complex web layouts. This tool was built to provide:

- A unified library and command-line utility for metadata, content, and structured tabular data extraction.
- Automatic domain-bounded site navigation with cycle prevention.
- Automated identification and verification of Algerian domain extensions (`.dz`), regional telephone numbering plans, and official business identifiers.

---

## 3. Key Capabilities

- **Automated Metadata & Content Parsing:** Extracts core OpenGraph attributes, canonical links, semantic heading hierarchies (`h1`-`h4`), and sanitized article paragraphs.
- **Tabular Data Transformation:** Parses arbitrary HTML tables into structured lists of keyed objects.
- **Targeted Querying:** Supports both CSS selector expressions and XPath queries for precise element retrieval.
- **Autonomous Site Crawling:** Built-in multi-page crawler with configurable depth limits, internal path discovery, request politeness delays, and visited-set cycle prevention.
- **Regional Telephony & Registry Verification:**
  - Validates `.dz` ccTLD registration and DNS records (nameservers, MX records, PTR).
  - Identifies mobile, landline, and national numbering formats across Algeria.
  - Recognizes administrative and fiscal registry numbers (NIF, NIS, RC, AI) and wilaya designations.
- **Multi-Format Serialization:** Exports extracted data cleanly into structured JSON, formatted Markdown, or console-friendly text.
- **Flexible Integration:** Operates as both an interactive CLI utility and a reusable Python module.

---

## 4. Technologies Used

- **Language:** Python 3 (3.8+)
- **Core Scraping Engine:** Scrapling (modern high-speed HTML parser)
- **Networking & DNS:** Requests, standard Python socket and DNS libraries
- **Data Serialization:** Standard library JSON, Markdown formatters
- **Testing:** Python unittest suite

---

[← Return to Project Portfolio](../README.md)
