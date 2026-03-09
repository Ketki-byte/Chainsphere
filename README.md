ChainSphere Backend

This is the backend API for the ChainSphere project, built with Node.js and Express. It manages user authentication, database interactions using Prisma, and integrates Web3 functionalities.

✨ Features

*   User Authentication: Handles user registration, login, password management (including forgot/reset password functionality), and session management.
*   Web3 Integration: Contains controllers and utilities for interacting with blockchain networks (Ethereum-compatible), likely for managing addresses and transactions.
*   Database Management: Uses Prisma as an ORM to interact with a database (configuration in the `prisma/` folder).
*   RESTful API: Organized routes and controllers for different resources like users, addresses, and admin functions.
*   Security: Implements authentication middleware to protect routes, uses environment variables for sensitive data, and has examples for secure password handling.

🛠️ Tech Stack

*   Runtime: Node.js
*   Framework: Express.js
*   Database ORM: Prisma
*   Language: JavaScript
*   Web3 Library: Likely `web3.js` or `ethers.js` (inferred from `Web3/` directory)

🚀 Getting Started

Prerequisites :

*   Node.js (v18 or higher recommended)
*   npm or yarn
*   A database (PostgreSQL, MySQL, etc.) supported by Prisma

Installation :

1.  Clone the repository
   
    git clone https://github.com/Ketki-byte/Chainsphere.git
    cd Chainsphere


Install dependencies :

npm install
  or
yarn install

Set up environment variables
Copy the example environment file and update it with your configuration:

cp .env.example .env

Set up the database with Prisma :

npx prisma migrate dev --name init

📁 Project Structure

chainsphere

├── .github/workflows/   # GitHub Actions CI/CD workflows

├── controllers/         # Request handlers for different API routes

├── middlewares/         # Custom middleware functions (auth, validation, etc.)

├── prisma/              # Prisma schema and migration files

├── public/              # Static files (like temporary uploads)

├── routes/              # API route definitions

├── utils/               # Helper functions and utilities

├── view/                # (Possibly for server-side rendered views or emails)

├── Web3/                # Web3-specific logic and configurations

├── .env.example         # Example environment variables

├── index.js             # Main application entry point

└── package.json         # Project metadata and dependencies


