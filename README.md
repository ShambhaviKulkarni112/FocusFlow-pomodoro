# FocusFlow – Pomodoro Study Tracker

FocusFlow is a cute, pastel-themed Pomodoro + study tracker web app designed for students.  
It helps you run focus sessions, track what you studied, and visualize your progress with simple charts.

## Features

- Pomodoro timer with configurable Focus, Short Break, and Long Break durations  
- Cute pastel UI with a “kawaii dessert” aesthetic  
- Subject management (add, rename, delete subjects with color tags)  
- Automatic logging of completed focus sessions  
- Session history with filters (by subject and date range)  
- Stats section with total focus time and a bar chart for the last 7 days  
- CSV export of all session data  
- Optional backend (Node + Express) for storing subjects and sessions

## Tech Stack

- Frontend: HTML, CSS, JavaScript (no frameworks)  
- Charts: Lightweight JS chart library (via CDN) or custom canvas/SVG  
- Backend (optional): Node.js + Express with in-memory storage

## Getting Started (Frontend Only)

1. Clone or download this repository.  
2. Open `index.html` in your browser.  
3. Choose a subject, start a Focus session, and let the timer run.  
4. Check the Session History and Stats sections to see your logged time.

> Note: In some sandboxed environments (like online previews), persistent storage (localStorage or API) may be disabled.  
> The app will still work for the current session, but data may reset on reload.

## Running with Backend (Node + Express)

1. Install Node.js (if not already installed).  
2. In the project folder, install dependencies:


3. Start the backend server:

4. Open `index.html` in your browser.  
The frontend will attempt to talk to the backend API (e.g., `http://localhost:3000/api/...`).  
If the backend is not reachable, the app will fall back to in-memory data.

## Project Structure

.
├─ index.html # Main UI
├─ styles.css # Pastel UI styles
├─ script.js # Timer, subjects, sessions, stats, storage helpers
├─ server.js # Optional Node + Express backend
└─ package.json # Backend dependencies and scripts

## Usage Tips

- Adjust your Focus/Break durations in the settings panel.  
- Create different subjects for each course (e.g., DSA, OS, DBMS, Math).  
- Use the filters in Session History to review what you studied today, this week, or this month.  
- Export sessions as CSV if you want to analyze your study data elsewhere.

## Future Improvements

- User authentication and cloud sync  
- More detailed analytics (streaks, best study days, etc.)  
- Sound notifications and customizable themes

## License

This project is for learning and personal use.  
Feel free to fork and modify it for your own studies.
