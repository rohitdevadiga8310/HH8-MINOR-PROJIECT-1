# JWT Secure API with FastAPI

A high-security REST API built using **Python**, **FastAPI**, and **JSON Web Tokens (JWT)**.

Security Features
- **Short-Lived Access Tokens:** Tokens expire after **1 minute**. This significantly limits the time attackers have to use an intercepted token.
- **HS256 Encryption:** This is a secure signing algorithm that maintains data integrity.
- **Middleware Protection:** The system automatically verifies tokens on all sensitive endpoints.

Tools Used
- **Language:** Python 3.x
- **Framework:** FastAPI
- **Library:** PyJWT (for token encoding and decoding)
- **Documentation:** Swagger/OpenAPI (Built-in)

How to Run
1. **Clone the repository:**
   `git clone https://github.com/your-username/jwt-secure-api.git`
2. **Install Dependencies:**
   `pip install fastapi[all] PyJWT python-dotenv`
3. **Run the Server:**
   `python -m uvicorn main:app --reload`
4. **Access Swagger UI:**
   Open `http://127.0.0.1:8000/docs` to test the login and protected routes.

Usage Note
To test the 1-minute expiry:
1. Generate a token via the `/login` endpoint.
2. Use the token to access `/secure-data`.
3. Wait 61 seconds and try again. The API will return a `401 Unauthorized` status.
4. And last add screens

## Conclusion
This project provides a secure and scalable JWT authentication system using FastAPI.
It follows best practices for token handling and environment security.

## Output Verification

Open Swagger UI

Login to get token

Copy token

Test protected endpoint

Verify 401 Unauthorized without token

Verify 200 OK with tokenhot and past it for git hub


