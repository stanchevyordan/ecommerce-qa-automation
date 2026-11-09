# E-commerce Application – Test Scenarios

## 1. User Registration

| ID | Test Scenario | Expected Result |
|---|---|---|
| TS-001 | Verify registration with valid user details | A new account is successfully created. |
| TS-002 | Verify registration with an already registered email | The system prevents duplicate registration. |
| TS-003 | Verify registration with missing mandatory fields | The system displays appropriate validation messages. |
| TS-004 | Verify registration with an invalid email format | The system rejects the invalid email address. |

## 2. User Login

| ID | Test Scenario | Expected Result |
|---|---|---|
| TS-005 | Verify login with valid credentials | The user successfully logs in. |
| TS-006 | Verify login with an incorrect password | The system rejects the login attempt. |
| TS-007 | Verify login with an unregistered email | The system displays an appropriate error message. |
| TS-008 | Verify login with empty credentials | The system displays mandatory field validation. |

## 3. Product Catalog and Search

| ID | Test Scenario | Expected Result |
|---|---|---|
| TS-009 | Verify that the product catalog displays available products | Products are displayed correctly. |
| TS-010 | Search for a product using its exact name | Matching products are displayed. |
| TS-011 | Search for a product that does not exist | An appropriate no-results message is displayed. |
| TS-012 | Open a product details page | Correct product information is displayed. |

## 4. Shopping Cart

| ID | Test Scenario | Expected Result |
|---|---|---|
| TS-013 | Add a product to the shopping cart | The product is added successfully. |
| TS-014 | Add multiple products to the shopping cart | All selected products are displayed. |
| TS-015 | Remove a product from the shopping cart | The selected product is removed. |
| TS-016 | Update the quantity of a cart item | The quantity and total price are updated correctly. |

## 5. Checkout and Orders

| ID | Test Scenario | Expected Result |
|---|---|---|
| TS-017 | Complete checkout with valid information | The order is successfully placed. |
| TS-018 | Attempt checkout with missing mandatory information | The system prevents order placement. |
| TS-019 | Verify the order total before placing an order | The total price is calculated correctly. |
| TS-020 | Verify order history after successful checkout | The newly placed order appears in order history.