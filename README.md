# Project: JWT Secure API
**Objective:** Implement a secure API using JSON Web Tokens with short-lived expiration for high security.

### Features
- User Authentication (Login)
- JWT Generation (1-minute expiry)
- Protected Routes (Middleware verification)
- Interactive Documentation (FastAPI/Swagger)

### How to Run
1. Install dependencies: `pip install fastapi[all] PyJWT python-dotenv`
2. Start server: `python main.py`
3. Access UI: `http://127.0.0.1:8000/docs`