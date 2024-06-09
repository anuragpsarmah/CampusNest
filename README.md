# Setting up CampusNest

Follow the instructions below to setup CampusNest on your local machine.

## Prerequisites

Node.js must be installed on your system.

## Cloning the Repository

Clone the repository to your local machine:

```bash
git clone https://github.com/anuragpsarmah/CampusNest.git
cd CampusNest
```

## Backend Configuration

**Environment Files**: Navigate to the `backend` folder and create `.env` file. Add the following content to the file:

    ```plaintext
    MONGODB_CONNECTION_STRING=

    JWT_SECRET_KEY=
    FRONTEND_URL=

    # Cloudinary Variables
    CLOUDINARY_CLOUD_NAME=
    CLOUDINARY_API_KEY=
    CLOUDINARY_API_SECRET=

    # Stripe
    STRIPE_API_KEY=
    ```
    
 - Create accounts at MongoDB, CLoudinary and Stripe to setup the keys. `JWT_SECRET_KEY` can be any secret or randomly generated key.  
 - The `FRONTEND_URL` should point to the URL where the frontend application is running (typically `http://localhost:3000`).
  

## Frontend Configuration

**Environment Files**: Navigate to the `frontend` folder and create a file: `.env`:

    ```plaintext
    VITE_API_BASE_URL=
    VITE_STRIPE_PUB_KEY=
    ```
    
- The `VITE_API_BASE_URL` should point to the URL where the backend application is running (typically `http://localhost:7000`).

## Running the Application

1. **Backend**:
    - Navigate to the `backend` directory.
    - Install dependencies: `npm install`.
    - Start the server: `npm start`.

2. **Frontend**:
    - Open a new terminal and navigate to the `frontend` directory.
    - Install dependencies: `npm install`.
    - Start the frontend application: `npm run dev`.
    - The application should now be running on `http://localhost:5173`.
