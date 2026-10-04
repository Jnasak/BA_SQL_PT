# UAT Test Cases (Sample)

| TC ID | Related Story | Test Scenario | Steps | Expected Result | Priority |
|-------|---------------|---------------|-------|-----------------|----------|
| TC-01 | US-01 | View real-time inventory | 1. Login as Warehouse Supervisor<br>2. Search SKU "ELEC-1001" | System shows current available, reserved, and location quantities updated within last 60s | High |
| TC-02 | US-01 | Multi-location view | 1. Search SKU available in warehouse and Store #3 | Both locations and quantities displayed correctly | High |
| TC-03 | US-02 | CS order status lookup | 1. Login as CS Agent<br>2. Enter order number | Full status, item locations, and ETA shown | High |
| TC-04 | US-02 | Handle customer inquiry | Simulate customer call about delayed order | Agent can see exact reason and current location | High |
| TC-05 | US-03 | Mobile picking | 1. Login on scanner<br>2. Start assigned picking batch | Guided path by zone, scan confirmation required | High |
| TC-06 | US-03 | Picking productivity | Complete 10-order batch | System records time and accuracy | Medium |
| TC-07 | US-04 | Low stock alert | Reduce stock of top SKU below reorder point | Alert sent to Manager + suggested PO created | Medium |
| TC-08 | US-05 | Automatic allocation | Place new Express order with available stock | Order allocated within 5 minutes and appears in picking queue | High |
| TC-09 | US-06 | Exception dashboard | Force an order past promised ship date | Order appears on Exception Dashboard with reason | Medium |
| TC-10 | BR-08 | End-to-end integration | Place order on website → allocate → pick → ship | Inventory decremented correctly in all systems | High |
