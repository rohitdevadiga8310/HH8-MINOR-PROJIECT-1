# JWT Secure API with FastAPI

A high-security REST API implementation using **Python**, **FastAPI**, and **JSON Web Tokens (JWT)**.

 🔐 Security Features
- **Short-Lived Access Tokens:** Tokens are set to expire in **1 minute**, significantly reducing the window of opportunity for attackers if a token is intercepted.
- **HS256 Encryption:** Secure signing algorithm for data integrity.
- **Middleware Protection:** Automatic token verification on all sensitive endpoints.

## 🛠️ Tools Used
- **Language:** Python 3.x
- **Framework:** FastAPI
- **Library:** PyJWT (for token encoding/decoding)
- **Documentation:** Swagger/OpenAPI (Built-in)

## 🚀 How to Run
1. **Clone the repository:**
   `git clone https://github.com/your-username/jwt-secure-api.git`
2. **Install Dependencies:**
   `pip install fastapi[all] PyJWT python-dotenv`
3. **Run the Server:**
   `python -m uvicorn main:app --reload`
4. **Access Swagger UI:**
   Open `http://127.0.0.1:8000/docs` to test the login and protected routes.

## 📝 Usage Note
To test the 1-minute expiry:
1. Generate a token via the `/login` endpoint.
2. Use the token to access `/secure-data`.
3. Wait 61 seconds and try again; the API will return a `401 Unauthorized` status.