Here's your complete `README.md` file incorporating the additional sections you provided:

```markdown
# E-Commerce Store (MERN Stack)

## Description
This e-commerce store is a full-stack application built using the MERN stack (MongoDB, Express.js, React.js, Node.js). The application leverages third-party APIs to enhance its functionality and supports three main user flows:

- **Buyers:** Browse through store categories, products, and brands.
- **Sellers/Merchants:** Manage brand components, add/update/delete products, and monitor sales.
- **Admins:** Oversee the entire store, including user management, order processing, and inventory control.

## Features

- **Node.js:** Provides a robust backend environment for handling multiple requests and ensuring high performance.
- **Express.js:** Used as middleware to manage HTTP requests and routes, simplifying the development of a secure and scalable web application.
- **Mongoose Schemas:** Models the application data structure in MongoDB, ensuring consistency and providing powerful querying capabilities.
- **React.js:** Powers the frontend with reusable UI components for a dynamic and responsive user experience.
- **Redux:** Manages the application's state, offering a predictable state container that synchronizes state across different components.
- **Redux Thunk:** Middleware used to handle asynchronous operations within Redux, especially for managing API calls and data flow between frontend and backend.

## Quickstart Guide

To run this project locally, you can use Docker Compose provided in the repository. Here’s a guide on how to run this project locally using Docker Compose.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/ecommerce-store.git
   ```

2. **Edit the `dockercompose.yml` file** and update the values for `MONGO_URI` and `JWT_SECRET`.

3. **Start the Docker Compose:**
   ```bash
   docker compose -f dockercompose.yml up
   ```

## Database Seed

- The seed command will create an admin user in the database.
- The email and password are passed with the command as arguments.
- Replace brackets with your email and password in the command below.
- For more information, see code [here](server/utils/seed.js).

```bash
npm run seed:db [email-***@****.com] [password-******] 
```

## Demo

This application is deployed on Vercel. Please check it out :smile: [here](https://mern-store-gold.vercel.app).

See the admin dashboard [demo](https://mernstore-bucket.s3.us-east-2.amazonaws.com/admin.mp4).

## Installation

Some basic Git commands to install the project locally:

```bash
git clone https://github.com/yourusername/ecommerce-store.git
cd project
npm install
```

## Start Development

```bash
npm run dev
```

## Simple Build for Production

```bash
npm run build
```

## Run Build for Production

```bash
npm start
```

## Languages & Tools

- [Node](https://nodejs.org/en/)
- [Express](https://expressjs.com/)
- [Mongoose](https://mongoosejs.com/)
- [React](https://reactjs.org/)
- [Webpack](https://webpack.js.org/)

## Code Formatter

To ensure consistent code formatting, follow these steps:

1. Add a `.vscode` directory.
2. Create a file `settings.json` inside `.vscode`.
3. Install the Prettier - Code formatter in VSCode.
4. Add the following snippet to `settings.json`:

```json
{
  "editor.formatOnSave": true,
  "prettier.singleQuote": true,
  "prettier.arrowParens": "avoid",
  "prettier.jsxSingleQuote": true,
  "prettier.trailingComma": "none",
  "javascript.preferences.quoteStyle": "single"
}
```
```

This `README.md` provides clear instructions for setting up, running, and understanding the project, along with tools and formatting guidelines to maintain code quality. Replace placeholder information like URLs and credentials with your actual details.
