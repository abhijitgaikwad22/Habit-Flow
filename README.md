📋 HabitFlow — Detailed Project Description
🔍 What is HabitFlow?
HabitFlow is a full-stack habit tracking web application built with Python (Flask). It allows users to create personal accounts, define daily habits, track their completion streaks, view progress analytics, earn achievement badges, and export their data to Excel — all through a beautifully designed dark-themed UI.

🛠️ Tech Stack
LayerTechnologyBackendPython 3 + FlaskFrontendHTML5, CSS3, Jinja2 TemplatesData StorageJSON files (no database)Exportopenpyxl (Excel .xlsx)DeploymentGunicorn (production server)FontsGoogle Fonts (Plus Jakarta Sans, Sora)

🔑 Core Features
1. 👤 User Authentication

Register with a username and password
Login / Logout with session management
Password strength meter on registration
Profile photo upload support (PNG, JPG, GIF, WebP)

2. ✅ Habit Management

Add habits with title, category, frequency, notes, and a goal (in days)
Toggle completion — mark a habit done/undone for today
Delete habits
Filter by category (Health, Fitness, Learning, Work, Personal)
Search habits by name

3. 🔥 Streak Tracking

Automatically calculates the current streak for each habit
Tracks total completions ever
Shows best streak across all habits

4. 📊 Dashboard Analytics

Daily completion progress bar (e.g., 3/5 habits done today)
7-day bar chart showing weekly habit completion trends
Stats: total habits, done today, best streak, total check-ins ever

5. 📅 Calendar View

Per-habit 12-week calendar heatmap
Shows each day as done ✅ or missed
Highlights today's date

6. 🏆 Achievements System

8 unlockable badges based on real progress:

🌱 First Step — Add your first habit
🔥 On Fire — 3-day streak
⚡ Week Warrior — 7-day streak
💎 Diamond Habit — 30-day streak
🎯 Habit Builder — Track 5+ habits
💪 Half Century — 50 total check-ins
🏆 Century Club — 100 total check-ins
🌈 All Rounder — Habits in all 5 categories


Progress bar showing how many badges are unlocked

7. 📁 Profile Page

Shows join date, profile photo, top habits by streak
Category breakdown — how many habits per category and today's completion rate per category

8. 📤 Excel Export

Exports full habit data to a styled .xlsx file
Two sheets: Summary (all habits with stats) and Completion History (every check-in date)

*The Path Should Look Like*
📁 Project Structure
Habit-Flow/
├── app.py              # Flask backend — all routes & logic
├── habits.json         # Habit data stored per user
├── users.json          # User accounts & profile info
├── requirements.txt    # Flask, openpyxl, gunicorn
├── .gitignore
└── templates/
    ├── index.html       # Main dashboard
    ├── login.html       # Login page
    ├── register.html    # Registration page
    ├── profile.html     # User profile
    ├── achievements.html# Badges page
    └── calendar.html    # Per-habit calendar view

🚀 How to Run
bash
pip install -r requirements.txt
python app.py
# Visit http://localhost:5000
