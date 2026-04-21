Act as a senior full-stack developer and extend my existing IT portal by adding a new module called:

"IT Asset Management and Lease Management System"

Important:
This is an EXISTING system. Do NOT rebuild from scratch.
Only ADD new features and integrate with existing database, APIs, and UI.

---

OBJECTIVE

Add advanced IT Asset Management features including:

Asset Inventory
Asset Allocation
Department Budget Management
Approval Workflow
Lease Management
Lease Cost Tracking
Terms and Conditions
User-Level Asset Configuration Policy

---

1. ASSET INVENTORY MODULE

Add asset management into existing system.

Fields:

Asset ID
Asset Type
Brand
Model
Serial Number
Department
Status (Available, Assigned, Maintenance)
Purchase or Lease
Warranty Expiry

Features:

Search assets
Filter by department
Track asset history
QR code tagging support

---

2. ASSET ALLOCATION MODULE

Allow assigning assets to employees.

Fields:

Employee ID
Employee Name
Department
Asset ID
Issue Date
Return Date

Features:

Assign asset
Return asset
Transfer asset
Allocation history tracking

---

3. DEPARTMENT BUDGET MODULE

Add department-wise IT budget tracking.

Fields:

Department Name
Annual Budget
Used Budget
Remaining Budget
Financial Year

Add workflow:

Department Head can send budget request to Management

Management can:

Approve
Reject
Hold

Notifications must be sent to both sender and receiver.

---

4. APPROVAL AUTHORITY MATRIX

Add approval hierarchy system.

Example:

Team Lead → up to 50,000
Manager → up to 100,000
Department Head → up to 300,000
Management → unlimited

System must validate approvals based on amount.

---

5. USER LEVEL ASSET CONFIGURATION POLICY

Define which asset configuration can be assigned to which user level.

Fields:

User Level
Department
RAM
Processor
Storage
Budget Range

System must prevent assigning low configuration assets to high-level users.

---

6. LEASE MANAGEMENT MODULE

Track leased assets.

Fields:

Vendor Name
Lease Start Date
Lease End Date
Lease Price
Contract Duration
Agreement Number

---

7. LEASE COST MODULE

Track financial details of lease.

Fields:

Monthly Cost
Contract Duration
Maintenance Cost
Vendor Fee
Total Cost

Auto calculation:

Total Cost = Monthly Cost × Duration

---

8. TERMS AND CONDITIONS MODULE

Store contract rules.

Fields:

Contract ID
Vendor Name
Terms Title
Terms Description
Start Date
End Date
Penalty Clause
Maintenance Responsibility
Replacement Policy
Status

Add validation:

Asset cannot be assigned if contract is expired.

---

9. NOTIFICATIONS

Trigger notifications for:

Asset assignment
Budget request
Budget approval
Lease expiry
Contract expiry

---

10. AUDIT LOGS

Track all actions:

User
Action
Timestamp
IP Address

---

11. UI INTEGRATION (IMPORTANT)

Integrate new modules into existing UI.

Add new menu items:

Asset Management
Asset Allocation
Department Budget
Lease Management
Lease Cost
Terms & Conditions
Reports

Do NOT break existing UI.

---

12. DATABASE CHANGES

Extend existing database.

Add new tables:

assets
asset_allocation
lease_contracts
lease_cost
terms_conditions
department_budget
budget_requests
approval_matrix
asset_policy

Ensure proper foreign keys and relationships.

---

13. API EXTENSION

Extend existing APIs.

Add endpoints:

/assets
/asset/assign
/budget/request
/budget/approve
/lease
/lease-cost
/terms

Use existing authentication system.

---

14. SECURITY

Use existing auth system.

Ensure:

Role-based access
Input validation
Secure APIs

---

OUTPUT REQUIRED

Provide:

* Updated database schema changes
* New API endpoints
* Backend service logic
* UI integration approach
* Sample code snippets for integration

Ensure everything integrates smoothly with existing system without breaking current features.
