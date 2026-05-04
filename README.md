# Project Scheduler Application

A Next.js application for scheduling projects and optimizing tasks based on cost and value.

## Features

- User management system
- Project creation with budget and schedule details
- Task management within projects
- Task optimization algorithm (knapsack problem)
- MongoDB database for persistent storage

## Technologies Used

- Next.js 15+
- React 19+
- MongoDB/Mongoose
- Tailwind CSS

## Setup Instructions

1. Clone the repository
2. Install dependencies:
   ```
   npm install
   ```
3. Set up MongoDB:
   - Make sure MongoDB is installed and running locally, or
   - Use MongoDB Atlas for cloud hosting
   - Copy `.env.example` to `.env.local` and update the MongoDB connection string

4. Run the development server:
   ```
   npm run dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser

## API Routes

- `/api/users` - GET all users, POST new user
- `/api/projects` - GET all projects, POST new project
- `/api/projects/:id` - GET, DELETE, PATCH specific project
- `/api/projects/:id/tasks` - POST new task to project
- `/api/projects/:id/tasks/:taskId` - DELETE, PATCH specific task

## Project Structure

- `/app` - Next.js app directory
- `/app/api` - API routes
- `/app/Components` - React components
- `/app/models` - MongoDB models
- `/app/lib` - Utility functions

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
