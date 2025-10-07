# 🍋 Mango Garden Estate Management System (MGEMS)

**Client Request Assessment (CRA) Report**  
**Prepared For:** CSE213 OOP Project  
**Prepared By:** Group31  
**Members:** [2432008, 2430825, 2430794, 2430936]

---

## 📌 Project Overview
The **Mango Garden Estate Management System (MGEMS)** simulates the operations of a mango estate, including:
- Field management
- Harvesting
- Inventory tracking
- Customer orders & sales
- Financial tracking
- Full Dashboard and Overview

The system demonstrates **Object-Oriented Programming (OOP)** principles such as **encapsulation, modularity, and interaction between objects (users)**.

---

## 👥 Users
- **Admin (Owner):** Oversees the estate and manages users
- **Manager (General Manager):** Plans tasks and monitors field operations
- **Field Supervisor:** Assigns and monitors daily tasks for workers
- **Worker (Gardener):** Performs field tasks and reports progress
- **Customer:** Places and tracks orders
- **Accountant:** Tracks sales, expenses, and wages
- **Sales Manager:** Handles customer orders, deliveries, and feedback
- **Warehouse Manager:** Manages inventory and dispatch of mangoes

---

## 🛠️ Event Types
- **UIE:** User Input Event
- **UID:** User Input Data
- **VL:** Validation Check
- **VR:** Verification Check
- **DP:** Data Processing
- **OP:** Output Display

---

## 🔄 Key Processes

### 1. Task Assignment (Manager → Supervisor → Worker)
- Manager assigns tasks → Supervisor delegates to Workers
- Events: `UIE, UID, VL, DP, OP`

### 2. Task Execution & Reporting (Worker → Supervisor → Manager)
- Workers complete tasks & report → Supervisor summarizes → Manager reviews
- Events: `UIE, UID, DP, OP`

### 3. Financial Tracking (Accountant)
- Record sales & expenses, calculate wages, generate reports
- Events: `UID, VL, VR, DP, OP`

### 4. Inventory Management (Warehouse Manager)
- Update stock, track spoilage, approve dispatch, generate reports
- Events: `UID, DP, VL, OP`

### 5. Customer Orders & Delivery (Customer → Sales Manager → Warehouse Manager)
- Customers place orders → Sales Manager confirms & tracks → Warehouse Manager prepares dispatch
- Events: `UIE, UID, DP, OP, VR`

---

## 🎯 User Goals & Workflows (Examples)

### Admin
- **Add/Remove Users:** Enter details → Validate → Save → Confirm
- **View Estate Summary:** Fetch data → Display report
- **Approve Expenses:** Review → Approve/Reject → Notify requester
- **Generate Reports:** Select period → Aggregate data → Display

### Manager
- **Assign Tasks:** Select field & worker → Enter details → Save → Notify Supervisor
- **Schedule Irrigation/Harvest:** Validate date → Save → Notify Supervisor
- **Track Completion:** Fetch supervisor reports → Display summary
- **Monitor Delivery Schedules:** Fetch from Sales Manager → Display

### Field Supervisor
- **Assign Daily Tasks:** Assign workers → Validate → Save → Notify
- **Record Attendance:** Mark → Save → Notify Manager
- **Report Field Issues:** Enter issue → Save → Notify Manager
- **Supervise Harvesting:** Record harvest data → Save → Notify

### Worker
- **View Assigned Tasks:** Fetch & display
- **Mark Complete:** Select task → Save → Notify Supervisor
- **Record Harvest Details:** Enter qty & quality → Save
- **Submit Daily Work Summary:** Summarize → Save → Notify Supervisor

### Customer
- **Place Order:** Validate → Save → Confirm
- **Track Order:** Enter ID → Fetch → Display
- **Make Payment:** Validate → Save → Confirm
- **Provide Feedback:** Save → Notify Sales Manager

### Accountant
- **Record Income/Expenses:** Enter → Save → Confirm
- **Track Payments:** Fetch pending → Display
- **Generate Reports:** Aggregate → Display
- **Calculate Wages:** Fetch attendance → Calculate → Save

### Sales Manager
- **Manage Customer Orders:** Confirm orders → Save → Notify Warehouse Manager
- **Track Deliveries:** Enter order ID → Fetch → Display
- **Record Delivery Completion:** Mark delivered → Save → Notify Customer
- **Handle Customer Feedback:** Collect → Save → Notify Admin

### Warehouse Manager
- **Receive Harvests:** Enter batch info → Save → Confirm
- **Update Stock:** Adjust qty → Save → Confirm
- **Track Spoilage:** Enter damaged qty → Save
- **Generate Inventory Report:** Aggregate → Display

---


### 📜 License
This project is for **educational purposes** under CSE213 OOP Project.
