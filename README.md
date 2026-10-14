# Web Application Security Project - OWASP Top 10

This project is a required part of the Introduction to Cyber Security MOOC course. The repository contains a vulnerable web application designed to demonstrate five different flaws from the OWASP Top 10 (2021) list, along with their corresponding fixes.
- [Flaw 1: Cryptographic Failures](https://github.com/aiki0/Securing-Software-Project-1/blob/main/config.py
)
- [Flaw 2: Identification and Authentication Failures](https://github.com/aiki0/Securing-Software-Project-1/blob/main/app.py#L396-L400
)
- [Flaw 3: Security Misconfiguration](https://github.com/aiki0/Securing-Software-Project-1/blob/main/app.py#L22-L27
)
- [Flaw 4: Security Logging and Monitoring Failure](https://github.com/aiki0/Securing-Software-Project-1/blob/main/app.py#L426-L427
)
- [Flaw 5: Vulnerable and Outdated Components](https://github.com/aiki0/Securing-Software-Project-1/blob/main/requirements.txt
)

Fixes for these flaws are commented out in the code
## Installation and Running Instructions

### For macOS / Linux

1. **Clone the repository:**

   ```bash
   git clone https://github.com/aiki0/Securing-Software-Project-1.git
   cd Securing-Software-Project-1
   ```

2. **Create and activate a Python virtual environment:**

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install the required dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Create the database and insert the initial data:**

   ```bash
   sqlite3 database.db < schema.sql
   sqlite3 database.db < init.sql
   ```

5. **(Optional) Prepare for testing the Flaw 1 fix:**
   Create an environment file to hold your custom secret key.

   ```bash
   cp .env.example .env
   ```

6. **Start the Flask application:**

   ```bash
   flask run
   ```

   The application will be accessible in your browser at `http://127.0.0.1:5000`.