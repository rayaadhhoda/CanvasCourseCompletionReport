# CanvasCourseCompletionReport
Here is a **clean, simple, copy-paste-ready README** formatted for GitHub.

No fluff — just the essentials.

---

# Canvas Course Completion Dashboard

This tool analyzes Canvas gradebook CSV files and generates:

* A **students-only** completion report
* A **dashboard-style summary** (overall + per course)
* A **deduplicated** student list across all CSVs
* A **downloadable CSV** of processed results

Everything runs **entirely in the browser** — no server, no installation.

---

## Features

### ✔ Students Only

Rows are included only if:

```
Role = StudentEnrollment
```

Teachers, TAs, Designers, and Observers are ignored.

---

### ✔ Deduplication

Students appearing in multiple files are merged using:

1. SIS User ID
2. SIS Login ID
3. Student Name (fallback)

---

### ✔ Completion Status

Each student is classified as:

* **Completed** – score recorded for every assignment
* **Started but not complete** – some scores, but at least one missing
* **Not started** – no scores recorded

Assignment columns are automatically detected between:

```
Section → Assignments Current Points
```

---

### ✔ Dashboard Summary

After uploading CSVs, the tool displays:

* **Overall totals** (unique students, completed, started, not started)
* **Per-course summary cards**
* **A scrollable detailed student table**

---

### ✔ CSV Export

You can download a consolidated CSV containing:

* Student name
* SIS User ID
* SIS Login ID
* Source file
* Completion status

---

## How to Use

1. Open `canvas_course_completion_dashboard.html` in any modern browser.
2. Click **Choose Files** and select one or more Canvas gradebook CSVs.
3. Click **Generate Completion Dashboard**.
4. View summaries and detailed results.
5. Click **Download Report as CSV** to save the processed data.

---

## File Overview

```
canvas_course_completion_dashboard.html   # Main dashboard tool
README.md                                 # Documentation
```

---

## Notes

* Everything runs locally — no data leaves your machine.
* Tool supports any number of CSV uploads.
* Designed for Canvas standard gradebook exports.

---

If you want charts, grouping features, or a hosted version, they can be added easily.
