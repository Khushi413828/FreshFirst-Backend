
# Fresh First – Business and Integrity Rules

## 1. Purpose

This document defines the business rules that Fresh First must follow to maintain accurate perishable stock records.

## 2. Mandatory Business Rules

### R1 – Expiry Date Rule
- A product whose expiry date is earlier than today's date must be identified as expired.
- Expired products must receive Critical priority.
- The recommended action must be Dispose.

### R2 – Near-Expiry Rule
- Products approaching their expiry date must be identified using the near-expiry threshold configured for their category.
- Near-expiry products must receive an appropriate priority.

### R3 – Valid Expiry Rule
- A product's expiry date must be later than its purchase date.
- Invalid date combinations must be rejected.

### R4 – Quantity Rule
- Product quantity must be a positive whole number.
- Zero, negative and decimal quantities must be rejected.

### R5 – Storage Temperature Rule
- Product storage temperature must be checked against the permitted temperature range of its category.
- Products outside the permitted range must be identified as having a storage issue.

### R6 – Mandatory Field Rule
- Required product information must not be empty.
- Incomplete product records must be rejected.

### R7 – Data Consistency Rule
- Product records must maintain valid category references.
- Invalid data must not be saved in the database.
- Failed database operations must not leave incomplete transactions.

## 3. Expected System Behaviour

| Rule | Expected Behaviour |
|---|---|
| R1 | Identify expired products |
| R2 | Identify near-expiry products |
| R3 | Reject invalid date combinations |
| R4 | Reject invalid quantities |
| R5 | Identify storage temperature issues |
| R6 | Reject missing mandatory fields |
| R7 | Maintain database consistency |

## 4. Validation Responsibility

The Flask backend is responsible for validating product information before database operations.

The database is responsible for maintaining relational integrity through appropriate constraints and relationships.

Testing is required to confirm that invalid inputs are rejected and valid records are stored correctly.

## 5. Expected Result

Fresh First must maintain accurate product information, identify expiry and storage issues, reject invalid inputs and preserve database integrity.
