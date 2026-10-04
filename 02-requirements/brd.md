# Business Requirements Document (BRD)  
## NovaMart – Order Fulfillment & Inventory Visibility Initiative

**Version:** 1.1  
**Status:** Approved  
**Business Analyst:** [Your Name]  
**Sponsor:** Marcus Lee (COO)  
**Date:** October 2025

---

### 1. Document Control

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 0.9 | 2025-09-15 | BA | Initial draft |
| 1.0 | 2025-09-28 | BA | Stakeholder review updates |
| 1.1 | 2025-10-05 | BA | Final approval |

---

### 2. Business Objectives

1. Reduce average order cycle time (order placement → shipment) from 4.8 days to **≤ 2.0 days**.
2. Increase inventory accuracy to **≥ 98%**.
3. Reduce stock-out rate on top 200 SKUs from 18% to **≤ 6%**.
4. Improve order accuracy to **≥ 98.5%**.
5. Provide real-time inventory visibility across online and physical stores.

---

### 3. Scope

**In Scope**
- Inventory Management System (IMS) selection & implementation
- Real-time stock synchronization between e-commerce, POS, and warehouse
- Warehouse process redesign (receiving, put-away, picking, packing, shipping)
- Exception management dashboards
- Training and change management for warehouse and customer service teams

**Out of Scope**
- Complete ERP replacement
- New e-commerce platform
- Supplier portal development (Phase 2)
- Advanced demand forecasting AI (future phase)

---

### 4. Stakeholders

See `01-discovery/stakeholder-register.md`

---

### 5. Business Requirements

| ID | Requirement | Priority | Source | Success Measure |
|----|-------------|----------|--------|-----------------|
| BR-01 | System shall provide real-time inventory levels across all channels | Must | COO, Warehouse | Inventory accuracy ≥ 98% |
| BR-02 | System shall support barcode / RFID scanning for all warehouse movements | Must | Warehouse | 100% scanned transactions |
| BR-03 | System shall automatically allocate stock to online orders based on rules | Must | Operations | Allocation time < 5 min |
| BR-04 | Customer Service shall be able to view real-time order & inventory status | Must | CS Manager | CS handle time reduced 20% |
| BR-05 | System shall generate picking lists optimized by zone and priority | Should | Warehouse | Picking productivity +30% |
| BR-06 | System shall support multi-location inventory (warehouse + stores) | Must | COO | Single source of truth |
| BR-07 | Managers shall receive automated alerts for low stock and delayed orders | Should | Operations | Proactive issue resolution |
| BR-08 | System shall integrate with existing e-commerce platform and POS | Must | IT | Seamless data flow |

---

### 6. Assumptions & Constraints

**Assumptions**
- Existing e-commerce platform has available APIs
- Warehouse staff will receive adequate training
- Budget of $420k is approved

**Constraints**
- Go-live target: within 7 months
- Must work with current network infrastructure
- Minimal disruption to daily operations during rollout

---

### 7. High-Level Risks

See Business Case document.

---

### 8. Approval

| Role | Name | Signature | Date |
|------|------|-----------|------|
| Project Sponsor | Marcus Lee | | |
| IT Director | Elena Rossi | | |
| Head of Warehouse | Priya Sharma | | |
| Business Analyst | | | |
