# To-Do App with Calendar View 📝

A modern, single-page web application for seamless task management, featuring an interactive calendar and a sleek interface. Built with **HTML**, **CSS**, and **JavaScript**, this app runs entirely client-side, using **FullCalendar** for dynamic calendar views, **SheetJS** for exporting tasks, and **localStorage** for persistent storage. Hosted on GitHub Pages, it’s lightweight, responsive, and perfect for personal or team productivity.

[![Live Demo](https://img.shields.io/badge/Live-Demo-blue?style=for-the-badge)](https://aayush0605.github.io/To-Do-Web-Application/)  
![GitHub repo size](https://img.shields.io/github/repo-size/aayush0605/To-Do-Web-Application)  
![GitHub last commit](https://img.shields.io/github/last-commit/aayush0605/To-Do-Web-Application)  
![License](https://img.shields.io/github/license/aayush0605/To-Do-Web-Application)

## 🚀 Features

### 📝 Task Manager
- **Create Tasks**: Add tasks with name, date, time, category (Work, Personal, Other), and priority (High, Medium, Low).
- **Edit & Delete**: Modify or remove tasks with ease; includes undo functionality for deletions.
- **Filters & Search**: Filter tasks by **All**, **Today**, or **Upcoming**, and search by name for quick access.
- **Task Status**: Track completion with checkboxes; tasks persist across sessions via `localStorage`.
- **Export Options**: Download tasks as **Excel** or **TXT** files, including status (Overdue, Today, Upcoming) and summaries.

### 📅 Calendar View
- **Interactive Calendar**: Powered by FullCalendar, view tasks on a monthly, weekly, or daily grid; click dates to filter tasks.
- **Table Calendar Fallback**: A custom table-based calendar (Sun-Sat layout) ensures functionality if the FullCalendar CDN fails.
- **Month Navigation**: Browse previous/next months in the table calendar.
- **Color-Coded Events**: Tasks are color-coded: red (overdue), yellow (today), green (upcoming).

### 🎨 Additional Features
- **Dark Mode**: Toggle between light and dark themes for comfortable viewing.
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices.
- **Pagination**: Navigate long task lists with Previous/Next buttons.
- **Stats Dashboard**: Displays total tasks, today’s tasks, and completed tasks.
- **Robust Error Handling**: Sanitizes inputs to prevent XSS and gracefully handles CDN failures.

## 🎥 Live Demo

Try the app now: [https://aayush0605.github.io/To-Do-Web-Application/](https://aayush0605.github.io/To-Do-Web-Application/)

## 🖼️ Screenshots

| Task Manager (Light Mode) | Calendar View (Dark Mode) |
|---------------------------|---------------------------|
| ![Task Manager](screenshots/task-manager-light.png) | ![Calendar View](screenshots/calendar-dark.png) |

*Note*: Add screenshots to the `screenshots/` folder in the repository and update paths if needed.

## 🛠️ Setup Instructions

### Run Locally
1. **Clone or Download**:
   ```bash
   git clone https://github.com/aayush0605/To-Do-Web-Application.git
   cd To-Do-Web-Application
   ```
   Or download the ZIP from [the repository](https://github.com/aayush0605/To-Do-Web-Application).

2. **Open the App**:
   - Double-click `index.html` to run in your browser (Chrome, Firefox, or Edge recommended).
   - *Optional*: Use a local server for better testing:
     ```bash
     npm install -g http-server
     http-server
     ```
     Access at `http://localhost:8080`.

3. **Test Features**:
   - Add a task (e.g., "Meeting" on 2025-09-11 at 14:00).
   - Switch between FullCalendar and table calendar views.
   - Filter tasks, toggle dark mode, and export to Excel/TXT.
   - Verify tasks persist after refreshing the page.

### Deploy to GitHub Pages
1. **Create/Update Repository**:
   - If not already done, ensure `index.html` is in the repo root: [github.com/aayush0605/To-Do-Web-Application](https://github.com/aayush0605/To-Do-Web-Application).
   - Upload `index.html` via **Add file** > **Upload files** and commit.

2. **Enable GitHub Pages**:
   - Go to **Settings** > **Pages** in the repository.
   - Set **Source**: **Deploy from a branch**, Branch: `main`, Folder: `/ (root)`.
   - Save. The site will be live at [https://aayush0605.github.io/To-Do-Web-Application/](https://aayush0605.github.io/To-Do-Web-Application/) within 1-10 minutes.

3. **Verify**:
   - Visit the URL and test all features (task creation, calendar, exports, etc.).
   - Check browser console (F12) for any errors.

## 📚 Usage

1. **Add a Task**:
   - Enter task details (name, date, time, category, priority) in the Task Manager.
   - Click **Add Task** to save. Tasks appear in the list and calendar.
2. **View Tasks**:
   - Use the **Task Manager** list or click dates in the **Calendar View** to filter tasks.
   - Switch between FullCalendar and table calendar using view buttons.
3. **Manage Tasks**:
   - Checkboxes mark tasks as completed.
   - Edit or delete tasks via buttons; deletions can be undone via notifications.
4. **Filter & Search**:
   - Use **All**, **Today**, or **Upcoming** buttons to filter.
   - Type in the search bar to find tasks by name.
5. **Export Data**:
   - Click **Export Excel** or **Export TXT** to download task data.
6. **Toggle Theme**:
   - Click **Toggle Dark Mode** for light or dark theme.

## 🐛 Troubleshooting

- **Calendar Not Loading**:
  - Check internet connection for CDN (`https://cdn.jsdelivr.net/npm/fullcalendar@6.1.15`).
  - The app falls back to the table calendar automatically. For a permanent fix, host FullCalendar locally:
    ```html
    <script src="./fullcalendar/main.min.js"></script>
    <link href="./fullcalendar/main.min.css" rel="stylesheet"/>
    ```
    Download files from [fullcalendar.io](https://fullcalendar.io/releases) and upload to a `fullcalendar/` folder.
- **Site Not Loading (404)**:
  - Ensure repo is public and `index.html` is in the root.
  - Verify GitHub Pages settings (Settings > Pages).
- **Buttons Not Working**:
  - Open console (F12 > Console) for JavaScript errors.
  - Use a modern browser (Chrome, Firefox, Edge; latest versions).
- **Jekyll Issues**:
  - Add an empty `.nojekyll` file to disable Jekyll:
    ```bash
    touch .nojekyll
    git add .nojekyll
    git commit -m "Disable Jekyll"
    git push
    ```
- **Limits**: GitHub Pages allows 1GB repo size and 100GB/month bandwidth (sufficient for this app).

See [SETUP_GUIDE.md](SETUP_GUIDE.md) for detailed contributor instructions.

## 🤝 Contributing

1. Fork the repository: [github.com/aayush0605/To-Do-Web-Application](https://github.com/aayush0605/To-Do-Web-Application).
2. Create a branch: `git checkout -b feature/your-feature`.
3. Commit changes: `git commit -m "Add feature"`.
4. Push: `git push origin feature/your-feature`.
5. Open a pull request with a clear description.

Please test changes locally and follow coding standards (consistent indentation, comments).

## 💻 Tech Stack

- **HTML/CSS/JavaScript**: Core web technologies for structure, styling, and interactivity.
- **FullCalendar (v6.1.15)**: Interactive calendar via CDN.
- **SheetJS**: Excel export functionality via CDN.
- **localStorage**: Client-side storage for task persistence.

## 📜 License

MIT License. See [LICENSE](LICENSE) for details.

## 📬 Contact

For issues, suggestions, or feedback, open a GitHub issue at [github.com/aayush0605/To-Do-Web-Application/issues](https://github.com/aayush0605/To-Do-Web-Application/issues).

---

**Get organized with style!** Try the To-Do App with Calendar View and boost your productivity. 🚀