# 📡 API Testing Assignment – Simple Books API

This repository contains the Postman collection and environment used to test the [Simple Books API](https://simple-books-api.glitch.me) as part of an API Testing assignment.

---

## 🔧 Tools Used

- [Postman](https://www.postman.com/) – for API testing
- GitHub – for version control and sharing

---

## 📁 Files Included

- `API-Testing-Assignment.postman_collection.json`: Postman Collection containing all 9 endpoint requests.
- `Simple-Books-Env.postman_environment.json`: Postman Environment file with saved variables (e.g., `accessToken`).

---

## ✅ Tested Endpoints

1. `GET /status` – Check API status  
2. `GET /books` – Retrieve list of books  
3. `GET /books/:bookId` – Get book details by ID  
4. `POST /orders` – Create a new order *(requires Bearer token)*  
5. `GET /orders` – View all orders *(requires Bearer token)*  
6. `GET /orders/:orderId` – View a specific order *(requires Bearer token)*  
7. `PATCH /orders/:orderId` – Update a specific order *(requires Bearer token)*  
8. `DELETE /orders/:orderId` – Delete a specific order *(requires Bearer token)*  
9. `POST /api-clients/` – Register API client to receive access token

---

## 💡 How to Use

1. Open Postman.
2. Import the collection and environment (`Import` → Upload both `.json` files).
3. Set the environment from the dropdown in the top-right.
4. Run the requests one by one using the access token generated via `POST /api-clients/`.
5. Token is automatically saved to `{{accessToken}}` using the Tests script.

---

## 📌 Note

- The access token is valid for **7 days**.
- If you get a `401 Unauthorized`, try generating a new token using a different email.

---



