# Simple User Authentication System

This is a basic user authentication system built with HTML, CSS, and JavaScript. It allows users to create an account, log in, and log out, with data stored locally using the browser's `LocalStorage`. The interface is designed in Sinhala (Sri Lankan language) and provides a simple, responsive user experience.

## Features

- **Account Creation**: Users can create an account with a username and password (`create-account.html`).
- **Login**: Authenticate using the created credentials (`login.html`).
- **Dashboard**: Displays a welcome message upon successful login (`dashboard.html`).
- **Logout**: Clears the stored user data and redirects to the login page.
- **Local Storage**: User data is stored in the browser's `LocalStorage` (single-user mode).
- **Responsive Design**: Simple and clean UI, centered on the page with a modern look.

## Project Structure
├── create-account.html  # Page to create a new account
<br>
├── login.html          # Login page for authentication
<br>
├── dashboard.html      # Dashboard displayed after successful login
<br>
└── README.md           # Project documentation

---


## How It Works

1. **Create Account** (`create-account.html`):
   - Users enter a username and password.
   - If no account exists in `LocalStorage`, the data is saved under the `"user"` key.
   - Redirects to `login.html` after 2 seconds with a success message.
   - If an account already exists, an error message is shown.

2. **Login** (`login.html`):
   - Users input their credentials.
   - Validates against the data in `LocalStorage`.
   - On success, redirects to `dashboard.html` after 2 seconds.
   - On failure or if no data exists, displays an error message.

3. **Dashboard** (`dashboard.html`):
   - Shows a welcome message.
   - Includes a "Logout" link that clears `LocalStorage` and redirects to `login.html`.

## Prerequisites

- A modern web browser (Chrome, Firefox, Edge, etc.).
- No server-side setup required; runs entirely client-side.

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
