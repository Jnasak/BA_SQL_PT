# Process Modeling Summary

## As-Is Process (High Level)

1. Customer places order on website  
2. Order sits in queue until supervisor manually checks stock  
3. Supervisor prints paper picking list  
4. Picker walks warehouse with paper list  
5. Items brought to packing station  
6. Packer packs and creates shipping label  
7. Inventory updated at end of day in spreadsheet / old system  
8. Customer Service has limited visibility until shipment confirmation

**Pain Points:** Delays at allocation step, picking errors, no real-time stock, reactive customer communication.

---

## To-Be Process (High Level)

1. Customer places order → System automatically allocates stock (rules engine)  
2. Order appears in mobile WMS as prioritized picking task  
3. Picker uses scanner; system guides optimal path by zone  
4. Scan confirmation updates inventory in real time  
5. Packing station receives digital packing instructions  
6. Shipping label auto-generated  
7. Customer Service and managers see live status + exception alerts  
8. Low-stock alerts trigger replenishment workflow

**Expected Improvements:**  
- Allocation time: from hours → < 5 minutes  
- Picking productivity: +30%  
- Inventory accuracy: 91% → ≥ 98%  
- Proactive issue resolution

---

> **Note:** Detailed process maps (BPMN / flowchart) should be created in draw.io or Lucidchart and linked/stored in this folder.
