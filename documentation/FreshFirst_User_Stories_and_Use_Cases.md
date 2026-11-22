
# Fresh First – User Stories and Use Cases

## 1. Admin

### User Stories
- As an Admin, I want to log in securely so that I can access administrative features.
- As an Admin, I want to manage user accounts so that access is controlled.
- As an Admin, I want to configure category storage temperature ranges and near-expiry thresholds.
- As an Admin, I want to view stock and verification reports.

### Use Cases
- UC-01: Admin Login
- UC-02: Manage User Accounts
- UC-03: Configure Category Rules
- UC-04: View Reports
- UC-05: Logout

## 2. Store Manager

### User Stories
- As a Store Manager, I want to view available stock so that I can monitor products.
- As a Store Manager, I want to verify products so that expired, near-expiry and storage issues are identified.
- As a Store Manager, I want to review product priorities so that urgent products receive attention.
- As a Store Manager, I want to confirm or change recommended actions.
- As a Store Manager, I want to view verification and action history.

### Use Cases
- UC-06: View Stock
- UC-07: Verify Products
- UC-08: Review Product Priority
- UC-09: Confirm or Change Action
- UC-10: View History
- UC-11: Generate Reports
- UC-12: Logout

## 3. Staff

### User Stories
- As Staff, I want to log in securely so that I can access permitted features.
- As Staff, I want to add product details so that stock records remain updated.
- As Staff, I want to edit product information when corrections are needed.
- As Staff, I want to view available products and their details.
- As Staff, I want to search for products easily.

### Use Cases
- UC-13: Staff Login
- UC-14: Add Product
- UC-15: Update Product
- UC-16: View Products
- UC-17: Search Products
- UC-18: Logout

## 4. General Use Case Conditions

- Users must log in before accessing protected features.
- Each role must have only its permitted access.
- Invalid inputs must be rejected with suitable error messages.
- Database changes must be saved successfully before a success message is displayed.
