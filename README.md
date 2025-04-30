# 📚 Books API Testing - Postman Collection

This project demonstrates API testing using Postman for a Books Management system. It covers essential CRUD operations and authentication using bearer tokens. The collection is designed to validate the behavior of book listing, order placement, retrieval, updating, and deletion functionalities.

---

## 🚀 Project Objectives

- Authenticate client using Bearer Token
- Test endpoints for:
  - Listing books
  - Placing an order
  - Retrieving order details
  - Updating order details
  - Deleting an order
- Validate API behavior through automated test scripts and dynamic variable usage

---

## 🛠️ Technologies Used

- **Postman** – API testing tool
- **Postman Environment Variables** – For dynamic base URL, tokens, and order IDs
- **JavaScript Test Scripts** – For assertions and variable handling

---

## 📂 Collection Overview

### 🔐 Authentication
- **POST** `/api-clients/`
- Generates a bearer token using `clientName` and `clientEmail`

### 📚 Book Listing
- **GET** `/books`
- Lists all available books

### 📦 Orders
- **POST** `/orders/` — *Place a new order*
- **GET** `/orders/{{orderId}}` — *Get order details*
- **PATCH** `/orders/{{orderId}}` — *Update customer name*
- **DELETE** `/orders/{{orderId}}` — *Delete an order*

### 🔁 Utilities & Tests
- `RANDOM_DATA_PARSE_JSON_RESPONSE` – Tests dynamic customer names with status checks (including a deliberate fail)
- `SET_RESET_VALUE` – Demonstrates variable setting and resetting
- `to check Patch and delete` – Verifies PATCH/DELETE behavior with previously placed orders

---

## 🧪 Example Tests Included

- Assert response status codes (e.g., 200, 201,404...)
- Parse JSON response and set environment variables
- Dynamic customer name generation
- Deliberate fail test for error handling demonstration

---

## 👩‍💻 Author

**Hafsa Farhan**  
Software Engineering Student |QA Intern| 10Pearls Pakistan

---

## 📅 Date

30 April 2025

---
