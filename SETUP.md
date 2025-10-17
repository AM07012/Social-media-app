# MERN Social App Setup Guide

## Quick Start with MongoDB Atlas (Recommended)

### 1. Set up MongoDB Atlas (Free)

1. Go to [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
2. Sign up for a free account
3. Create a new project
4. Build a free cluster (M0 Sandbox)
5. Create a database user with username/password
6. Whitelist your IP address (or use 0.0.0.0/0 for development)
7. Get your connection string

### 2. Configure Environment Variables

Create a `.env` file in the project root with:

```env
# MongoDB Atlas Connection String
MONGODB_URI=mongodb+srv://yourusername:yourpassword@cluster.mongodb.net/mernproject?retryWrites=true&w=majority

# JWT Secret (use a secure random string)
JWT_SECRET=your_super_secret_jwt_key_here

# Server Configuration
PORT=3000
NODE_ENV=development
```

### 3. Install Dependencies (Already Done)
```bash
npm install
```

### 4. Run the Application
```bash
npm run development
```

## Alternative: Install MongoDB Locally

1. Download MongoDB Community Server from [mongodb.com/try/download/community](https://www.mongodb.com/try/download/community)
2. Install and start MongoDB service
3. Use the default connection string: `mongodb://localhost:27017/mernproject`

## Troubleshooting

- Make sure your MongoDB connection string is correct
- Ensure your IP is whitelisted in MongoDB Atlas
- Check that the database user has read/write permissions
- Verify that the database name is `mernproject`

## Application Features

- User authentication (signup/signin)
- User profiles
- Create and view posts
- Like and comment on posts
- Follow/unfollow users
- User search

## Access the App

Once running, visit: http://localhost:3000

