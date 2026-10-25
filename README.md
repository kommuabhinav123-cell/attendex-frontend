# 🎨 Attendex Frontend Documentation & Structure

All client-side files, UI layouts, styling, and templates are consolidated in this directory.

```
frontend/
├── static/
│   ├── css/
│   │   └── style.css            # Custom Attendex styles & color theme
│   ├── js/
│   │   └── app.js               # Alerts dismissal & DOM helpers
│   └── images/                  # Visual assets & logos
└── templates/
    ├── index.html               # Main landing page (Home, Features, About, Contact)
    ├── login.html               # Role-based login portal (Admin, Faculty, Student)
    ├── register.html            # Student self-registration form
    ├── fragments/
    │   └── layout.html          # Reusable top navbar, meta head, and footer
    ├── admin/
    │   ├── dashboard.html       # Admin KPI dashboard
    │   ├── students.html        # Students directory with search & filters
    │   ├── student-form.html    # Add student form
    │   ├── student-edit.html    # Edit student profile
    │   ├── faculty.html         # Faculty directory & status toggles
    │   ├── faculty-form.html    # Add faculty form
    │   ├── departments.html     # Academic departments management
    │   ├── courses.html         # Course management
    │   ├── sections.html        # Class sections (CS-A, etc.)
    │   ├── subjects.html        # Course subjects
    │   ├── assignments.html     # Faculty class mapping
    │   ├── enrollments.html     # Student subject enrollments
    │   └── reports.html         # Attendance filtering & CSV export
    ├── faculty/
    │   ├── dashboard.html       # Faculty assigned classes overview
    │   ├── mark-attendance.html # Attendance marking interface
    │   ├── view-attendance.html # Session log viewer & inline editor
    │   ├── sessions.html        # Session history & date filter
    │   └── low-attendance.html  # Defaulters list (< 75% attendance)
    ├── student/
    │   ├── dashboard.html       # Student percentage KPIs & defaulter banner
    │   ├── profile.html         # Student academic details & password change
    │   └── subject-attendance.html # Detailed subject attendance logs
    └── error/
        └── error.html           # Friendly error page
```

> **Note on Spring Boot Integration**: In Spring Boot applications, the runtime classpath looks in `src/main/resources/templates` and `src/main/resources/static`. This `frontend/` folder provides a clean, self-contained view of all UI assets for frontend development and version control.
