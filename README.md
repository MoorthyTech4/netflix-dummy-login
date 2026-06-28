# Netflix Login Clone

A full-stack clone of the Netflix login page, built with React on the frontend and Express on the backend. Includes form validation, mock authentication, and a redirect to a dummy dashboard on successful login.

## Features

- Netflix-style dark login UI with background image and red accent branding
- Email and password input fields with controlled state
- Frontend validation for empty fields, shown inline under each input
- Login form data sent to the backend via Axios
- Mock credential checking on the backend (no database)
- Error messages displayed for invalid login attempts
- Redirect to a dummy Dashboard page on successful login
- Sign out button on the dashboard that returns to the login page

## Tech Stack

**Frontend:** React, Vite, React Router DOM, Axios, Tailwind CSS

**Backend:** Node.js, Express, CORS

## Usage

Start the backend server:

```
cd backend
npm install
npm start
```

The backend runs on `http://localhost:5000`.

Start the frontend in a separate terminal:

```
cd frontend
npm install
npm run dev
```

The frontend runs on `http://localhost:5173`.

Demo credentials:

```
Email: test@netflix.com
Password: password123
```

or

```
Email: admin@netflix.com
Password: admin123
```

## Error Handling

- If the email or password field is left empty, an inline error appears under the relevant field and the request is not sent.
- If the backend receives a request with missing fields, it responds with a 400 status and an error message.
- If the email and password do not match any mock user, the backend responds with a 401 status and an "Invalid email or password" message, which is displayed above the form.
- If the backend is unreachable or an unexpected error occurs, a generic error message is shown instead.
