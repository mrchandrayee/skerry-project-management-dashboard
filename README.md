# skerry — Project Management Dashboard

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?style=for-the-badge&logo=github)](https://mrchandrayee.github.io/skerry-project-management-dashboard/)
[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org) [![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org) [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](./LICENSE)

A runnable responsive project-management frontend reconstructed from the supplied 6.07-second screen recording.

## Run locally
1. Extract `skerry-project-management-dashboard.zip`.
2. Open `index.html` in Chrome, Firefox, Safari or Edge.

No npm install or build step is required.

Optional local server:
```bash
python3 -m http.server 8000
```
Open `http://localhost:8000`.

## Screens recreated
- **Dashboard:** Total Projects 18, Ended Projects 6, Running Projects 9, Pending Project 3; weekly project analytics chart; North Mole design-review reminder; project mini-list; recent activity and progress.
- **Projects:** Cards and table views, All / In review / In progress / Delivered filters, project search, progress bars, team avatars, create project and log-time forms.
- **Tasks:** Kanban columns To do, In progress, Checking and Done; task cards, search, create task, drag-and-drop status updates and CSV export.
- **Calendar:** Week view with sample project events.
- **Analytics:** Hours logged, tasks completed, on-time delivery, team utilisation, weekly bar chart and project status breakdown.
- **Team:** Team member directory.
- **Settings:** Workspace, email notifications, task reminders and weekly digest toggles.
- **Help:** Support request demo.
- Collapsible sidebar / rail mode, dark-light theme, global search, notification and message feedback, responsive mobile navigation.

## Source code fragment visible in the video
The recording shows a `src/App.tsx` fragment for `toggleRail()` (roughly lines 1–16). It queries `.frame` and `.side`, reads the main and sidebar geometry, toggles `is-rail`, uses GSAP `fromTo` for the main x-position, then animates the sidebar `clipPath` from its expanded width to zero. The original project files are not fully visible. This vanilla JS project recreates that rail-collapse behaviour with CSS transitions and implements the visible screens and interactions; it is not a verbatim recovery of the original React/GSAP source.

## Demo data and limitations
All client, task, team and project records are local sample data. Forms update in-memory browser state only; refresh resets the demo. CSV export is implemented for tasks. No login, database, API, calendar sync, email, meeting provider or live team collaboration is connected.

## 👨‍💻 Author

**mrchandrayee** · [GitHub](https://github.com/mrchandrayee)

## 📄 License

[MIT License](./LICENSE)
