# ⚡ HabitFlow

> **Build habits · Track streaks · Grow daily**

HabitFlow is a full-stack **habit tracking web application** built with **Python (Flask)**. It allows users to create personal accounts, define daily habits, track completion streaks, view progress analytics, earn achievement badges, and export data to Excel — all through a beautifully designed dark-themed UI.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python 3 + Flask |
| Frontend | HTML5, CSS3, Jinja2 Templates |
| Data Storage | JSON files (no database) |
| Export | openpyxl (Excel .xlsx) |
| Deployment | Gunicorn (production server) |
| Fonts | Google Fonts (Plus Jakarta Sans, Sora) |

---

## 🔑 Core Features

### 👤 1. User Authentication
- Register with a username and password
- Login / Logout with session management
- Password strength meter on registration
- Profile photo upload support (PNG, JPG, GIF, WebP)

### ✅ 2. Habit Management
- Add habits with title, category, frequency, notes, and a goal (in days)
- Toggle completion — mark a habit done/undone for today
- Delete habits
- Filter by category (Health, Fitness, Learning, Work, Personal)
- Search habits by name

### 🔥 3. Streak Tracking
- Automatically calculates the current streak for each habit
- Tracks total completions ever
- Shows best streak across all habits

### 📊 4. Dashboard Analytics
- Daily completion progress bar (e.g., 3/5 habits done today)
- 7-day bar chart showing weekly habit completion trends
- Stats: total habits, done today, best streak, total check-ins ever

### 📅 5. Calendar View
- Per-habit 12-week calendar heatmap
- Shows each day as ✅ done or missed
- Highlights today's date

### 🏆 6. Achievements System

8 unlockable badges based on real progress:

| Badge | Icon | Requirement |
|---|---|---|
| First Step | 🌱 | Add your first habit |
| On Fire | 🔥 | Reach a 3-day streak |
| Week Warrior | ⚡ | Reach a 7-day streak |
| Diamond Habit | 💎 | Reach a 30-day streak |
| Habit Builder | 🎯 | Track 5 or more habits |
| Half Century | 💪 | Complete 50 total check-ins |
| Century Club | 🏆 | Complete 100 total check-ins |
| All Rounder | 🌈 | Have habits in all 5 categories |

### 👤 7. Profile Page
- Shows join date, profile photo, top habits by streak
- Category breakdown — habits per category and today's completion rate

### 📤 8. Excel Export
- Exports full habit data to a styled `.xlsx` file
- Two sheets: **Summary** (all habits with stats) and **Completion History** (every check-in date)

---

## 📁 Project Structure

```
Habit-Flow/
├── app.py                  # Flask backend — all routes & logic
├── habits.json             # Habit data stored per user
├── users.json              # User accounts & profile info
├── requirements.txt        # Flask, openpyxl, gunicorn
├── .gitignore
└── templates/
    ├── index.html          # Main dashboard
    ├── login.html          # Login page
    ├── register.html       # Registration page
    ├── profile.html        # User profile
    ├── achievements.html   # Badges page
    └── calendar.html       # Per-habit calendar view
```

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/abhijitgaikwad22/Habit-Flow.git
cd Habit-Flow

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the app
python app.py

# 4. Visit in your browser
# http://localhost:5000
```

---

## 💡 Future Improvements

- Switch from JSON to a real database (SQLite / PostgreSQL)
- Add password hashing (bcrypt) for security
- Email/reminder notifications
- Mobile app version
- Weekly/monthly habit reports

---

## 👨‍💻 Author

**Abhijit Gaikwad** — [@abhijitgaikwad22](https://github.com/abhijitgaikwad22)
