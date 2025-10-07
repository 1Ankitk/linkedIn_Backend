# LinkedIn Backend Platform

A **LinkedIn-style social networking backend** built using **Node.js**, **Express.js**, **MongoDB**, and **Neo4j**.  
This project enables secure authentication, user profile management, and graph-based relationship modeling for professional connections.

---

## 🚀 Features

- 🔐 **JWT Authentication**
  - Secure user login and registration using JSON Web Tokens.
  - Middleware-based route protection for all private APIs.

- 👥 **User Profiles**
  - Create, update, and fetch user profiles.
  - Manage profile details and account settings.

- 🌐 **Graph-Based Connections (Neo4j)**
  - Store and query professional relationships (connections, mutuals, suggestions).
  - Efficient traversal of the social graph using Cypher queries.

- 📦 **Modular Express Architecture**
  - Follows controller–service–model separation for clean, maintainable code.
  - Centralized error handling and validation middleware.

- ⚙️ **Scalable & Configurable**
  - Environment-based configuration for DB credentials and JWT secrets.
  - Supports deployment on platforms like Render, Railway, or GCP.

---

## 🏗️ Tech Stack

| Layer | Technologies |
|-------|---------------|
| **Backend Framework** | Node.js, Express.js |
| **Databases** | MongoDB, Neo4j |
| **Authentication** | JWT |
| **ORM / ODM** | Mongoose |
| **Environment Management** | dotenv |
| **Version Control** | Git & GitHub |

---

## 📁 Project Structure

```
linkedIn_Backend/
├── controllers/
│ └── users.js
├── models/
│ └── users.js
├── routes/
│ └── users.js
├── service/
│ └── auth.js
├── middleWares/
│ └── auth.js
├── database.js
├── neo4jDb.js
├── connect.js
├── index.js
├── package.json
└── README.md
```
---

## ⚡ Getting Started

1.  **Clone the repository:**
    ```
    git clone https://github.com/1Ankitk/linkedIn_Backend.git
    cd linkedIn_Backend
    ```

2.  **Install dependencies:**
    ```
    npm install
    ```

3.  **Set up environment variables** - Create a `.env` file in the root directory:
    ```
    PORT=5000
    MONGO_URI=your_mongodb_connection_string
    NEO4J_URI=your_neo4j_bolt_uri
    NEO4J_USER=your_neo4j_username
    NEO4J_PASSWORD=your_neo4j_password
    JWT_SECRET=your_secret_key
    ```

4.  **Run the server:**
    ```
    npm start
    ```
    The server will start at `http://localhost:5000`.

---

## 📈 Future Enhancements

- 🔍 Search and recommendations for "People You May Know"
- 💬 Messaging and real-time notifications
- 📄 File uploads for profile pictures and resumes
- 📊 Analytics dashboard for user activity

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to modify.
