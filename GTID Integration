# GTID Integration and MIR Linkage — Professional Documentation

Welcome to the **GTID Integration Knowledge Base**. This page documents the integration of GTIDs in Smartpoint, along with MIR device linkage and key host commands. It is designed for professional reference and can be published directly as a GitHub Page.

---

## 📌 GTID Assignment Table

| Client ID | PCC  | Host | GTID   | Type                       | Ordinal | TINIT | TCTY | Status    | Notes                 |
|-----------|------|------|--------|----------------------------|---------|-------|------|-----------|-----------------------|
| gdm5xnjq  | 88SQ | 1G   | F702F9 | PRT - Plain Paper/OPTAT    | 2       | BOMOU | DEL  | Complete  | Assigned GTID: F702F9 |
| gdm5xnjq  | 88SQ | 1G   | F702FA | PRT - Plain Paper/OPTAT    | 3       | BOMOU | DEL  | Complete  | Assigned GTID: F702FA |

---

## 🔗 Linkage Notes

To generate a **MIR (Miscellaneous Information Record)** successfully, you must be linked to a MIR device.

### Key Host Commands

#### HMET — Display Electronic Ticket Support Document Print Table
- `HMET`

#### Link / Delink Terminal to MIR GTID
- **Link terminal:** `HMLMF72203DA` → Links terminal to MIR GTID F72203  
- **Delink terminal:** `HMLM/DELINK/A` → Delink from MIR device only

#### Designate Printer for Stock Type
- **Ticketing:** `HMOMF72303–TKT` → Designate printer for ticketing
- **Itinerary/Invoice:** `HMOMF92304–ITN` → Designate printer for itinerary/invoice
- **Blank Stock:** `HMOMF32303–BLK` → Designate printer for blank stock

#### Change Printer Status
- **Set printer UP:** `HMOMF82303–U`
- **Set printer DOWN:** `HMOMF82303–D`

#### Display Linkage
- **Display linkage of terminal:** `HMLD`
- **Display linkage for all terminals in PCC XC7:** `HMLDXC7`

---

## 📂 Quick Reference — Example Codes

- `HMLMF702F9DIE/F702FADT` → Linkage for specific GTID F702F9
- `HMOMF702F9-U` → Printer status UP for GTID F702F9
- `HMOMF702FA-U` → Printer status UP for GTID F702FA
- `HMOMF702F9-ITN` → Itinerary printer designation for GTID F702F9
- `HMOMF702FA-TKT` → Ticketing printer designation for GTID F702FA

---

## ✅ Best Practices
- Always confirm linkage (`HMLD`) before attempting to generate a MIR.
- Ensure each GTID has the correct **ticketing** and **itinerary printer** configured.
- Use `HMET` frequently to verify support document table status.
- When troubleshooting, check:
  - Printer designation (TKT / ITN / BLK)
  - Printer status (UP/DOWN)
  - MIR linkage status

---

## 📘 Glossary
- **GTID:** Galileo Terminal Identifier
- **MIR:** Miscellaneous Information Record (used for reporting)
- **PCC:** Pseudo City Code
- **TKT:** Ticketing stock
- **ITN:** Itinerary/invoice stock
- **BLK:** Blank stock

