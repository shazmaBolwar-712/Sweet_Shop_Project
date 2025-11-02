# Sweet_Shop_Project
The Sweet Shop Management System is a full-stack web application designed to efficiently manage sweet inventory, purchases, and user roles (Admin &amp; User). It provides a clean and modern interface for managing sweets, viewing stock, purchasing items, and performing administrative actions like adding, updating, deleting, and restocking sweets.

**User Features**

Register and Login as a user or admin.

View available sweets and filter/search them by name or category.

Purchase sweets (quantity decreases automatically).

Responsive and user-friendly dashboard.

**Admin Features**

Add new sweets with name, category, price, and quantity.

Edit or delete existing sweets.

Restock items (quantity increases).

Manage the entire inventory with secure admin access.

**Authentication** 

JWT-based authentication for secure access.

Role-based routing (separate dashboards for Admin and User).

Password hashing using bcrypt.

Forgot Password and Reset Password functionality with secure email links.

**Tech Stack Layer Technology**

Used Frontend React, TypeScript, TailwindCSS, Axios, React Router Backend Node.js, Express.js, Prisma ORM Database PostgreSQL Authentication JWT, bcryptjs Email Service Nodemailer (Gmail App Password) Testing Jest (for API tests)


**System Architecture Frontend**

(React + Axios) 
↓
 Backend (Express + Prisma) 
↓ 
PostgreSQL Database

**Project Setup Guide**

Prerequisites

Make sure you have installed:

Node.js (v18+)

PostgreSQL

npm or yarn

Git

Backend Setup

Navigate to the backend folder

cd backend

Install dependencies

npm install

Create the .env file

DATABASE_URL="postgresql://postgres:yourpassword@localhost:5432/sweetshop" JWT_SECRET="supersecretkey123" EMAIL_USER="your_email@gmail.com" EMAIL_PASS="your_gmail_app_password"

Run Prisma migrations

npx prisma migrate dev --name init

Start the backend

npm run dev

Your backend should now be running at http://localhost:5000

Frontend Setup

Navigate to the frontend folder

cd frontend

Install dependencies

npm install

Start the frontend

npm run dev

Your frontend will run at http://localhost:5173

Running Tests

You can run backend API tests using Jest or Postman.

Example Test Commands npm test

Test Coverage Includes:

User registration and login

Role-based access verification

CRUD operations for sweets

Purchase and restock actions

**Test Report Example Output**

PASS tests/auth.test.js ✓ should register user ✓ should login as admin ✓ should reject invalid password PASS tests/sweet.test.js ✓ should add sweet ✓ should update quantity after purchase ✓ should delete sweet (admin only)

**My AI Usage**

In this section, I describe how AI tools assisted me throughout the development process.

Tools used

ChatGPT (GPT-5 by OpenAI)

Perplexity 

**How i used them**

I used ChatGPT extensively during the planning and development stages:
To generate and refine the Express.js routes for authentication and sweets CRUD.
To debug Prisma migration errors and design a consistent database schema.
To help create clean and reusable React components for login, register, and dashboards.
For generating setup documentation and project explanation (this README section).
Auto-completing small code snippets inside React forms.
Suggesting Tailwind class combinations to improve UI consistency.
Writing repetitive try-catch structures and axios calls.

**Reflection on AI Impact**

AI tools significantly improved my productivity:

They reduced development time by helping me debug Prisma, Node, and frontend state errors faster.

The generated code was accurate, and I learned best practices for authentication and REST API design.
However, I ensured that I understood and verified every AI suggestion — editing logic, handling security, and customizing UI manually.

Overall, AI acted as a technical assistant, not a replacement. It enhanced my learning and allowed me to deliver a polished, functional project efficiently.

**Conclusion**

The Sweet Shop Management System showcases a well-structured full-stack application featuring role-based authentication, efficient inventory management, and a smooth user experience. It highlights modern web development practices by seamlessly integrating performance, usability, and security.
