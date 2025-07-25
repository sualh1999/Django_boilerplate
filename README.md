# Django Auth Boilerplate API

This is a basic Django authentication API with signup, login, and logout endpoints.

## Setup

1.  **Create a virtual environment and activate it:**

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

2.  **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

3.  **Run database migrations:**

    ```bash
    python3 manage.py migrate
    ```

4.  **Run the development server:**

    ```bash
    python3 manage.py runserver
    ```

## API Endpoints

*   **Signup:** `POST /api/auth/signup/`
    *   **Send:** `username`, `password`
    *   **Receive:** `id`, `username`

*   **Login:** `POST /api/auth/login/`
    *   **Send:** `username`, `password`
    *   **Receive:** `token`

*   **Logout:** `POST /api/auth/logout/`
    *   **Send:** `Authorization: Token <your_token>` header
    *   **Receive:** `204 No Content`
