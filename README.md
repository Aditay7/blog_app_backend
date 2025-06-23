# Blogging Application

A full-stack blogging platform built with Node.js, Express, MongoDB, and EJS. Users can register, sign in, create blog posts with image uploads, comment on posts, and browse all blogs.

## Features

- User registration and authentication (JWT-based, passwords hashed)
- Blog post creation with image upload (Multer)
- Commenting on blog posts
- Homepage listing all blogs with cover images
- Individual blog view with comments
- EJS templating for dynamic HTML rendering
- Static file serving for images and uploads

## Technologies Used

- Node.js, Express.js
- MongoDB, Mongoose
- EJS (views)
- Multer (file uploads)
- JWT (authentication)
- dotenv (environment variables)

## Project Structure

```
├── app.js                # Main server file
├── models/               # Mongoose schemas (User, Blog, Comment)
├── routes/               # Express routers (user, blog)
├── middlewares/          # Authentication middleware
├── services/             # JWT token logic
├── views/                # EJS templates (pages and partials)
├── public/               # Static assets (images, uploads)
├── .env.example          # Example environment variables
├── package.json          # Project metadata and scripts
```

## Getting Started

### Prerequisites

- Node.js and npm
- MongoDB instance (local or cloud)

### Installation

1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd <project-directory>
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set up environment variables:
   - Copy `.env.example` to `.env` and fill in your MongoDB connection string and desired port.

### Running the App

- Start the server:
  ```bash
  npm start
  ```
- For development with auto-reload:
  ```bash
  npm run dev
  ```
- Visit [http://localhost:8000](http://localhost:8000) (or your configured port)

## Environment Variables

- `MONGO_URL`: MongoDB connection string
- `PORT`: Port for the server (default: 8000)

## Scripts

- `npm start`: Runs the app
- `npm run dev`: Runs the app with nodemon

## License

ISC
