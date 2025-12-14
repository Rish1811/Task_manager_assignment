# Task Manager App

This is a simple task management application built with React, inspired by Trello. It allows users to create, edit, delete, and drag/drop tasks across three boards: To-Do, In-Progress, and Completed. Data is persisted using localStorage, and initial tasks are loaded from a JSON file.

## Setup

1. Clone the repository:
 git clone <your-repo-url>
 cd task-manager-app
2. Install dependencies:
 npm install react-beautiful-dnd dayjs --legacy-peer-deps

3. Start the development server:
   npm start

The app will be available at `http://localhost:3000`.

## Scripts

- `npm start`: Runs the app in development mode.
- `npm run build`: Builds the app for production.
- `npm test`: Runs tests (if any).

## Folder Structure

- `public/`: Static assets (index.html, favicon, etc.).
- `src/`
- `components/`: Reusable components (TaskModal.js, Filters.js).
- `App.js`: Main application component.
- `App.css`: Global styles.
- `tasks.json`: Initial tasks data.
- `index.js`: Entry point.
- `package.json`: Dependencies and scripts.
- `README.md`: This file.

## Features

- Responsive 3-column board layout (To-Do, In-Progress, Completed).
- Add/edit tasks via modal with title, description, priority, due date, status.
- Drag-and-drop to move tasks between boards (updates status instantly).
- Filters: Priority, Due Date (by date), Status.
- Sorting: Newest/Oldest First, Closest Due Date.
- Delete with confirmation; duplicate title handling (appends (1), etc.).
- Loads from tasks.json; persists to localStorage.
- Classic UI with vanilla CSS.

Built with React, react-beautiful-dnd (for drag-drop), dayjs (for dates).

## Deployment

### GitHub Pages
1. Install gh-pages: `npm install --save-dev gh-pages`
2. Add to `package.json` (in "homepage" field): `"homepage": "https://<your-username>.github.io/task-manager-app"`
3. Add to "scripts": `"predeploy": "npm run build", "deploy": "gh-pages -d build"`
4. Run: `npm run deploy`
5. Enable GitHub Pages in repo settings > Pages > Source: Deploy from gh-pages branch.

### Vercel/Netlify
- Push to GitHub first (steps below).
- Connect repo to Vercel/Netlify dashboard; auto-deploys on push.

Live Demo: [Insert your live URL here after deployment]
