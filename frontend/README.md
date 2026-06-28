Netflix Login Clone

A full-stack clone of Netflix's sign-in page, built with React and Express.js, featuring form validation and a mock authentication flow.

Features


Netflix-style login UI built with React and Tailwind CSS
Client-side form validation (Gmail format check, password rules)
Inline error messages for invalid email/password input
Mock backend authentication with Express.js
CORS-enabled API for cross-origin requests between frontend and backend
Responsive layout for mobile and desktop
Deployed on Vercel (frontend and backend as separate projects)


Tech Stack

Frontend


React (Create React App)
React Router DOM
Tailwind CSS v3
Axios
Context API for auth state management


Backend


Node.js
Express.js (ESM modules)
CORS middleware


Deployment


Vercel (monorepo with separate frontend/backend projects)
Deployment Notes

This project is deployed as two separate Vercel projects from the same monorepo:


Frontend — Root Directory set to frontend, Framework Preset: Create React App
Backend — Root Directory set to backend, Framework Preset: Other


The frontend communicates with the backend via its stable Vercel domain (not the deployment-specific URL, which changes on every deploy).