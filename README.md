# 📦 Procure-to-Pay (P2P) – Full Purchasing Cycle in SAP MM

> **SAP BTP Academic Project** | B. Tech CSE | KIIT University
> 
> A complete end-to-end documentation of the Procure-to-Pay process implemented in SAP Materials Management (SAP MM), submitted as part of the SAP Business Technology Platform (BTP) Programme.

---

## 👤 Author Details

| Field | Details |
|---|---|
| **Name** | Saurav Kumar |
| **Roll Number** | 23053524 |
| **Program** | SAP BTP |
| **Branch** | B. Tech CSE |
| **Batch** | 2023 – 2027 |
| **Submission Date** | 19th April 2026 |

---

## 📋 About This Project

This project documents the **Procure-to-Pay (P2P)** business process as implemented in **SAP SD/MM/FI** modules. The P2P cycle covers the complete journey from an internal purchase request all the way to the final vendor payment — one of the most critical workflows in any enterprise ERP system.

The report was prepared as per the **KIIT SAP Project Work Guidance**, following the end-to-end scenario format with step-by-step process documentation, real SAP transaction screenshots, process flow diagrams, and technical analysis.

---

## 🔄 P2P Process Flow

```
┌─────────────────────────────────────────────────┐
│           PROCURE-TO-PAY (P2P) CYCLE            │
└─────────────────────────────────────────────────┘

  [ME51N] Purchase Requisition
         ↓  Auto Trigger
  [ME41]  Request for Quotation
         ↓  Auto Trigger
  [ME21N] Purchase Order
         ↓  Auto Trigger
  [MIGO]  Goods Receipt
         ↓  Auto Trigger
  [MIRO]  Invoice Verification  (3-Way Match)
         ↓  Auto Trigger
  [F110]  Automatic Payment Run
         ↓
  ✅ Cycle Complete — Vendor Paid & Cleared in SAP
```

---

## 🗂️ Report Structure

| Section | Title |
|---|---|
| 1 | Title & Introduction |
| 2 | Process Flow Diagram |
| 3 | Problem Statement |
| 4 | Solution / Features (Step-by-Step P2P) |
| 5 | Screenshots (SAP GUI Transactions) |
| 6 | Tech Stack |
| 7 | Unique Points |
| 8 | Future Improvements |
| 9 | Conclusion |

---

## 🛠️ SAP Transactions Covered

| Step | T-Code | Description |
|---|---|---|
| 1 | `ME51N` | Create Purchase Requisition |
| 2 | `ME41` | Request for Quotation |
| 3 | `ME21N` | Create Purchase Order |
| 4 | `MIGO` | Post Goods Receipt |
| 5 | `MIRO` | Vendor Invoice Verification (3-Way Match) |
| 6 | `F110` | Automatic Payment Run |

---

## 🧰 Tech Stack

| Technology | Role |
|---|---|
| **SAP MM** | Materials Management — core P2P orchestration |
| **SAP FI** | Financial Accounting — AP, GR/IR, payment |
| **SAP SD** | Sales & Distribution — demand-driven procurement |
| **SAP ECC 6.0 / S/4HANA** | ERP platform |
| **SAP GUI** | Transaction interface |
| **SAP BTP** | Business Technology Platform — programme context |

---

## 📁 Repository Contents

```
📂 sap-p2p-project/
├── 📄 README.md                     ← You are here
└── 📄 sap_p2p_report_23053524.docx  ← Full Project Report (Word Document)
```

---

## 🔑 Key Concepts Demonstrated

- **Three-Way Match** — Automatic reconciliation of PO, Goods Receipt & Invoice
- **Document Flow** — Full traceability from Requisition to Payment
- **Release Strategy** — Configurable approval workflows for spending control
- **Real-Time FI Integration** — Every goods movement posts to accounting instantly
- **Automated Payment** — F110 payment run with due-date logic and bank clearing

---

## 📌 Topic Reference

This project follows **Topic (i)** from the KIIT SAP Project Work Guidance:

> *Procure-to-Pay (P2P) — Full Purchasing Cycle (SAP MM)*

---

## 📜 Disclaimer

This project is submitted for academic purposes as part of the **KIIT SAP BTP Programme**. All SAP screenshots used are sourced from publicly available SAP tutorial resources for educational demonstration.
