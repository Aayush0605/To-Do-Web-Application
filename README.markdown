# To-Do App with Calendar View

A sleek, single-page web app for managing tasks with an interactive calendar, built with HTML, CSS, and JavaScript. Hosted on GitHub Pages, it uses FullCalendar for a modern calendar view, SheetJS for exporting tasks, and `localStorage` for persistence. Features include task creation, filtering, dark mode, and Excel/TXT exports.

[![Live Demo](https://img.shields.io/badge/Live-Demo-blue?style=for-the-badge)](https://yourusername.github.io/your-repo-name/)
![GitHub repo size](https://img.shields.io/github/repo-size/yourusername/your-repo-name)
![GitHub last commit](https://img.shields.io/github/last-commit/yourusername/your-repo-name)

## Features

- **Task Management**: Add, edit, delete tasks with categories (Work, Personal, Other) and priorities (High, Medium, Low).
- **Calendar Views**: Toggle between FullCalendar (interactive) and table-based calendar with month navigation.
- **Filters & Search**: Filter tasks by All, Today, or Upcoming; search by task name.
- **Export Options**: Download tasks as Excel or TXT files with status and summaries.
- **Dark Mode**: Switch between light and dark themes for better usability.
- **Responsive Design**: Works seamlessly on desktop and mobile.
- **Persistence**: Tasks saved in browser `localStorage`.
- **Fallback**: Uses table calendar if FullCalendar CDN fails.

## Screenshots

| Task Manager (Light Mode) | Calendar View (Dark Mode) |
|---------------------------|---------------------------|
| ![Task Manager](screenshots/task-manager-light.png) | ![Calendar View](screenshots/calendar-dark.png) |

*(Screenshots placeholder: Add images to a `screenshots/` folder in the repo and update paths.)*

## Live Demo

Try the app at: [https://yourusername.github.io/your-repo-name/](https://yourusername.github.io/your-repo-name/)

## Setup Instructions

### Run Locally

1. Clone or download the repository:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   ```
   Or download the ZIP from GitHub.

2. Open `index.html` in a modern browser (Chrome, Firefox, Edge).
3. Test features: Add tasks, switch calendar views, filter, export, and toggle dark mode.

*Optional*: Use a local server for testing:
```bash
npm install -g http-server
cd your-repo-name
http-server
```
Visit `http://localhost:8080`.

### Deploy to GitHub Pages

1. Create a public repository on [GitHub](https://github.com).
2. Upload `index.html` to the repo root.
3. Go to **Settings** > **Pages**:
   - Source: **Deploy from a branch**.
   - Branch: `main`, Folder: `/ (root)`.
   - Save.
4. Access the site at `https://yourusername.github.io/your-repo-name/` (wait 1-10 minutes).

## Usage

1. **Add Task**: Enter task details (name, date, time, category, priority) and click "Add Task".
2. **View Tasks**: See tasks in the list or on the calendar (click dates to filter).
3. **Filter/Search**: Use buttons or search bar to narrow down tasks.
4. **Export**: Download tasks as Excel or TXT.
5. **Dark Mode**: Toggle theme for better visibility.
6. **Persistence**: Tasks save automatically in your browser.

## Troubleshooting

- **Calendar Not Loading**: Check internet for CDN access (`https://cdn.jsdelivr.net/npm/fullcalendar@6.1.15`). The app falls back to table calendar if the CDN fails.
- **Buttons Not Working**: Open console (F12) for errors. Ensure modern browser usage.
- **Site Not Live**: Verify repo is public, `index.html` is in root, and Pages is enabled.
- **Jekyll Issues**: Add `.nojekyll` file to disable Jekyll:
  ```bash
  touch .nojekyll
  git add .nojekyll
  git commit -m "Disable Jekyll"
  git push
  ```

## Contributing

1. Fork the repo.
2. Create a branch: `git checkout -b feature/your-feature`.
3. Commit changes: `git commit -m "Add feature"`.
4. Push: `git push origin feature/your-feature`.
5. Open a pull request.

See [SETUP_GUIDE.md](SETUP_GUIDE.md) for detailed contributor instructions.

## Tech Stack

- **HTML/CSS/JavaScript**: Core web technologies.
- **FullCalendar**: Interactive calendar (CDN).
- **SheetJS**: Excel export (CDN).
- **localStorage**: Client-side task storage.

## License

MIT License. See [LICENSE](LICENSE) for details.

## Contact

For issues or suggestions, open a GitHub issue or contact [your email or social link].

Happy task managing! 🚀