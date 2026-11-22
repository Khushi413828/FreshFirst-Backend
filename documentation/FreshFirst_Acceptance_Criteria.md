
# Fresh First – Acceptance Criteria

## 1. User Login

**Requirement ID:** FR-US-01

**Acceptance Criteria:**
- The user must be able to log in using valid credentials.
- Invalid credentials must be rejected with an appropriate error message.
- Passwords must not be stored or displayed as plain text.
- Users must access only the features allowed by their roles.

**Expected Result:** Login succeeds for valid credentials and fails for invalid credentials.

## 2. Add Product

**Requirement ID:** FR-ST-01

**Acceptance Criteria:**
- The user must be able to enter product details.
- Product name, category, quantity, purchase date and expiry date must be provided.
- Quantity must be a positive whole number.
- Expiry date must be later than purchase date.
- Invalid or incomplete product details must be rejected.
- Valid product details must be saved in the database.

**Expected Result:** Valid products are saved successfully, and invalid product entries are rejected with an appropriate message.

## 3. View Products

**Requirement ID:** FR-ST-03

**Acceptance Criteria:**
- The user must be able to view saved products.
- Product details must be displayed correctly.
- Archived products must not appear in the active stock list.
- The product list must show the correct quantity, category and expiry date.
- If no products are available, an appropriate message must be displayed.

**Expected Result:** The system displays the correct active product records from the database.

## 4. Update Product

**Requirement ID:** FR-ST-04

**Acceptance Criteria:**
- The user must be able to update an existing product.
- Updated product details must be validated before saving.
- Quantity must remain a positive whole number.
- Expiry date must be later than purchase date.
- Invalid updates must be rejected.
- Valid changes must be saved in the database.

**Expected Result:** The updated product details are saved correctly and displayed in the stock list.

## 5. Delete Product

**Requirement ID:** FR-ST-05

**Acceptance Criteria:**
- The user must be able to remove a product from the active stock list.
- The system must identify the correct product using its product ID.
- The product must be marked inactive instead of permanently deleting its record.
- Inactive products must not appear in the active stock list.
- The system must return an appropriate success or error message.

**Expected Result:** The selected product is archived successfully and no longer appears in active stock records.

## 6. Product Verification

**Requirement ID:** FR-VR-01 to FR-VR-07

**Acceptance Criteria:**
- The system must check the product expiry date.
- The system must identify expired and near-expiry products.
- The system must validate product quantity.
- The system must check storage temperature against the category's permitted range.
- Missing or invalid product information must be identified.
- The system must assign an appropriate verification status.
- Verification results must be saved in the database.

**Expected Result:** The system identifies product issues correctly and stores the verification result.

## 7. Priority Assignment

**Requirement ID:** FR-PR-01 to FR-PR-03

**Acceptance Criteria:**
- Expired products must receive Critical priority.
- Near-expiry products must receive an appropriate priority.
- Products with storage issues must receive an appropriate priority.
- Products with invalid or incomplete information must be marked for Inspection.
- Products without verification issues must receive Low priority.
- Priority must be displayed in the stock details.

**Expected Result:** Each product receives a priority based on its verification conditions.

## 8. Action Recommendation

**Requirement ID:** FR-AC-01 to FR-AC-04

**Acceptance Criteria:**
- The system must suggest an appropriate action based on product verification and priority.
- Expired products must receive a Dispose recommendation.
- Near-expiry products must receive an appropriate action such as Priority Sale, Quick Use or Redistribution.
- Products with storage issues or invalid information must receive an Inspection recommendation.
- The Store Manager must be able to confirm or change the suggested action.
- Confirmed actions must be saved in the database.

**Expected Result:** The system suggests suitable actions and stores the Store Manager's confirmed action.

## 9. History and Audit Trail

**Requirement ID:** FR-HS-01 to FR-HS-03

**Acceptance Criteria:**
- The system must record product verification activities.
- The system must record confirmed product actions.
- Each history record must include the activity, related product ID, user ID and activity timestamp.
- Authorized users must be able to view history records.
- Existing history records must not be modified or deleted through normal application operations.

**Expected Result:** Important verification and action activities are recorded with user and time details and can be reviewed later.

## 10. Reports

**Requirement ID:** FR-RP-01 to FR-RP-05

**Acceptance Criteria:**
- The system must generate stock reports.
- The system must display expired and near-expiry products.
- The system must display products with storage issues.
- The system must generate reports for products requiring attention.
- Users must be able to filter reports using available criteria.
- Reports must display accurate information from the database.
- Authorized users must be able to print or export reports if supported.

**Expected Result:** The system generates accurate reports using the available product and verification records.
