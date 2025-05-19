
# Multi-Tenant Event Management System

This project is a multi-tenant event management system built with Laravel 12 (backend) and Nuxt.js (frontend).

---

## Project Structure

```
/
├── backend/      # Laravel 12 API
├── frontend/     # Nuxt.js frontend
```

---

## Prerequisites

- PHP >= 8.2 (required for Laravel 12)
- Composer
- Node.js >= 18
- npm or yarn
- MySQL or any supported database

---

## Setup Instructions

### 1. Backend (Laravel 12 API)

```bash
cd event-management-api
composer install
npm install && npm run build
cp .env.example .env
# Update .env with your database credentials and other environment variables
php artisan key:generate
php artisan migrate
php artisan db:seed  # Optional, if you have seeders
php artisan serve
```

By default, Laravel will run on http://127.0.0.1:8000

---

### 2. Frontend (Nuxt.js)

Open a new terminal tab/window:

```bash
cd event-management-frontend
npm install      # or yarn install
npm run dev      # or yarn dev
```

Nuxt will run on http://localhost:3000 by default.

---

## Usage

- The frontend communicates with the backend API at http://127.0.0.1:8000.
- Make sure both backend and frontend servers are running simultaneously.
- Adjust API base URLs in the frontend config if needed.

---

## Additional Notes

- To build the frontend for production:
  ```bash
  npm run build
  npm run start
  ```
- To run backend tests:
  ```bash
  php artisan test
  ```

---

## Contact

For any questions or issues, please contact  cliffordmukosh@gmail.com or raise an issue in this repo.

---

Thank you for reviewing my project!
