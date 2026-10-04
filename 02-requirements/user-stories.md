# User Stories – NovaMart Order Fulfillment Project

All stories follow the **INVEST** criteria and include Gherkin-style acceptance criteria.

---

### Epic 1: Real-Time Inventory Visibility

**US-01**  
**As a** Warehouse Supervisor  
**I want** to see real-time stock levels for every SKU across warehouse and stores  
**So that** I can make accurate allocation and replenishment decisions  

**Acceptance Criteria:**
```gherkin
Given I am logged into the Inventory Management System
When I search for any SKU
Then I should see current available quantity, reserved quantity, and location
And the data should be updated within 60 seconds of any stock movement
```

**Priority:** Must  
**Story Points:** 8

---

**US-02**  
**As a** Customer Service Agent  
**I want** to view the exact status and inventory location of a customer’s order  
**So that** I can give accurate delivery promises and resolve issues quickly  

**Acceptance Criteria:**
```gherkin
Given a customer provides an order number
When I search the order in the system
Then I should see current status (Pending, Picking, Packed, Shipped, etc.)
And the warehouse location of each item
And estimated ship date
```

**Priority:** Must  
**Story Points:** 5

---

### Epic 2: Efficient Warehouse Operations

**US-03**  
**As a** Picker  
**I want** optimized picking lists grouped by warehouse zone  
**So that** I can pick more orders in less time with fewer errors  

**Acceptance Criteria:**
```gherkin
Given there are open orders ready for picking
When the system generates a picking batch
Then items should be grouped by zone and ordered by optimal path
And the list should be available on a mobile scanner device
```

**Priority:** Must  
**Story Points:** 13

---

**US-04**  
**As a** Warehouse Manager  
**I want** automatic low-stock alerts for top-selling items  
**So that** I can reorder before stock-outs occur  

**Acceptance Criteria:**
```gherkin
Given a SKU falls below its reorder point
When the inventory is updated
Then the system should send an alert to the Warehouse Manager and Purchasing team
And create a suggested purchase order draft
```

**Priority:** Should  
**Story Points:** 5

---

### Epic 3: Order Allocation & Exception Handling

**US-05**  
**As the** System  
**I want** to automatically allocate available stock to new online orders based on priority rules  
**So that** high-priority and older orders are fulfilled first  

**Acceptance Criteria:**
```gherkin
Given a new order is placed
When stock is available
Then the system allocates inventory within 5 minutes
And prioritizes Express orders and oldest orders first
```

**Priority:** Must  
**Story Points:** 8

---

**US-06**  
**As a** Customer Service Manager  
**I want** a dashboard of delayed and exception orders  
**So that** my team can proactively contact customers  

**Acceptance Criteria:**
```gherkin
Given orders that have missed their promised ship date
When I open the Exception Dashboard
Then I should see a prioritized list with customer contact details and reason codes
```

**Priority:** Should  
**Story Points:** 5
