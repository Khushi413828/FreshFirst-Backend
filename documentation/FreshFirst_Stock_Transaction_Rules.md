
# Fresh First – Stock Transaction Rules

## 1. Purpose

This document defines the types of stock-related transactions in Fresh First and explains how each transaction affects product quantity.

## 2. Transaction Types and Quantity Effects

| Transaction Type | Description | Effect on Stock Quantity |
|---|---|---|
| Stock Entry | Adding a new product with its initial quantity | Records the entered quantity |
| Stock Update | Updating an existing product's quantity | Replaces the previous quantity with the new quantity |
| Product Archive | Removing a product from active stock | No quantity deduction; product is marked inactive |
| Product Verification | Checking expiry, quantity and storage conditions | No quantity change |
| Action Recommendation | Suggesting disposal, sale, quick use or redistribution | No quantity change until an actual stock update is recorded |
| Product Search | Searching for available products | No quantity change |

## 3. Stock Integrity Rules

1. Product quantity must be a positive whole number during product entry.
2. Invalid or negative quantities must be rejected.
3. Product verification must not automatically change stock quantity.
4. Product archiving must not be treated as physical stock removal.
5. Only authorized users can perform permitted stock operations.
6. Product quantity must be saved correctly in the database.

## 4. Transaction Examples

| Example | Previous Quantity | Transaction | New Quantity |
|---|---:|---|---:|
| New product entry | 0 | Add 50 units | 50 |
| Quantity correction | 50 | Update to 40 | 40 |
| Product verification | 40 | Verify product | 40 |
| Product archive | 40 | Archive product | 40 (inactive) |

## 5. Current System Limitation

Fresh First currently maintains product quantity records and verification history. It does not yet maintain a complete stock movement ledger for every physical sale, disposal, consumption or redistribution.

Therefore, action recommendations alone do not deduct stock quantity.

## 6. Expected Result

The system must maintain valid product quantities, prevent invalid quantity entries and ensure that verification and recommendations do not unintentionally modify stock quantity.
