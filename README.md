# 🧩 User Management REST API with Flask

This is a simple **Flask REST API** that manages user data using basic CRUD operations — **Create, Read, Update, Delete**. It stores user info in an **in-memory list** (no database required).

---

## 📋 Features

* ✅ List all users (`GET /users`)
* ✅ Add a new user (`POST /users`)
* ✅ Update a user (`PUT /users/<id>`)
* ✅ Delete a user (`DELETE /users/<id>`)

---

## 🛠️ Tech Stack

* **Python 3**
* **Flask** (Web framework)
* **Postman / curl** (for testing)

---

## 🚀 Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/your-username/flask-user-api.git
cd flask-user-api
```

### 2. Install Dependencies

```bash
pip install Flask
```

### 3. Run the Application

```bash
python app.py
```

Server will start on:
📍 `http://127.0.0.1:5000/`

---

## 🔌 API Endpoints

### ➕ Create User

* **URL:** `POST /users`
* **Body (JSON):**

  ```json
  {
    "name": "Alice",
    "email": "alice@example.com"
  }
  ```
* **Response:**

  ```json
  {
    "id": 1,
    "name": "Alice",
    "email": "alice@example.com"
  }
  ```

---

### 📥 Get All Users

* **URL:** `GET /users`
* **Response:**

  ```json
  [
    {
      "id": 1,
      "name": "Alice",
      "email": "alice@example.com"
    }
  ]
  ```

---

### 📝 Update User

* **URL:** `PUT /users/<id>`
* **Body (JSON):**

  ```json
  {
    "name": "Alicia"
  }
  ```
* **Response:** Updated user object or 404 error

---

### ❌ Delete User

* **URL:** `DELETE /users/<id>`
* **Response:**

  ```json
  {
    "message": "User deleted"
  }
  ```

---

## 🧪 Testing

You can test the API using:

* 🧪 [**Postman**](https://www.postman.com/)
* 🧪 `curl` in the terminal

---

## 📁 File Structure

```
.
├── app.py         # Main Flask application
├── README.md      # Project documentation
```

---

## 📌 Notes

* This API uses **in-memory list** — all data will reset on server restart.
* Great for **learning**, **prototyping**, or **testing**.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---
