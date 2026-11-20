# Store Management & POS Accounting System

**GitHub Repository:** `kassiis/store-management-system`  
**Source code:** Private repository  
**Project Category:** Applications & Software Systems  
**Development Status:** Completed / Production-Ready System  

---

## 1. Overview

**Store Management & POS Accounting System** (نظام تسيير المحل) is a commercial point-of-sale, stock tracking, and financial reconciliation platform engineered for retail businesses in Algeria. The system blends a high-performance Python generation engine with an interactive, Right-to-Left (RTL) Arabic interface built upon Microsoft Excel and VBA automation.

---

## 2. Project Purpose

Small and medium retail establishments often encounter errors when attempting to track multi-partner equity, inventory shrinkage, supplier credit, and diverse Algerian payment channels (Cash, CCP, BaridiMob) using generic spreadsheet templates. This system delivers:

- A unified Arabic-first point-of-sale and inventory control workflow.
- Precise multi-partner accounting separating business expenses from owner capital withdrawals.
- Multi-channel cash drawer reconciliation matching physical cash with digital payment receipts.
- Programmatic generation, backup automation, and 15-point automated accounting validation.

---

## 3. Key Capabilities

- **13 Integrated Worksheets:** Comprehensive architecture encompassing:
  - **Live Dashboard:** Real-time revenue, margins, operating expenses, and inventory valuation KPIs.
  - **Inventory Catalog:** Real-time stock counts, cost-basis valuation, low-stock threshold alerts, and barcode indexing.
  - **Point of Sale (POS):** Fast barcode scanning, invoice line-item calculations, and cash vs. credit sale differentiation.
  - **Purchasing & Supplier Tracking:** Restocking invoice logs and supplier payment schedules.
  - **Inventory Adjustments:** Audit logs for damage write-offs, stock audits, and restorable customer returns.
  - **Operating Expenses:** Categorized cost ledger distinguishing paid from accrued operating costs.
  - **Treasury & Liquidity:** Multi-channel drawer closing tracking Cash, BaridiMob, CCP, and bank transfers.
  - **Multi-Partner Equity Accounts:** Capital contribution tracking, equity share calculations, and personal withdrawals isolated from operating overhead.
- **Python Automation Engine:** Custom Python scripts utilizing `openpyxl` to build, format, and style the entire 13-sheet workbook programmatically with native Excel formulas and conditional formatting.
- **Macro Integration (VBA):** Automated rapid barcode event triggers for instantaneous product lookup.
- **Automated Accounting Audit Suite:** Python-driven COM automation suite executing end-to-end integration tests verifying 15 realistic transaction scenarios (credit sales, debt settlement, returns, treasury balancing).
- **Archival & Backup Engine:** Automated backup utility providing file-integrity verification and timestamped snapshots.

---

## 4. Technologies Used

- **Core Automation Engine:** Python 3, `openpyxl`
- **Spreadsheet & UI Platform:** Microsoft Excel (XLSX / XLSM), VBA (Visual Basic for Applications)
- **Quality Assurance & Verification:** Python COM automation (`win32com.client`), unit testing suite
- **Localization:** Arabic RTL interface, ISO date conventions, Algerian Dinar (DZD) financial formatting

---

[← Return to Project Portfolio](../README.md)
