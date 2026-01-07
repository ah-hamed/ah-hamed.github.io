---
title: Grades WebApp with Flask
tags:
  - Webapp
  - Flask
date: 2023-04-26
hiddenInHomelist: true
TocOpen: true
---

**Grades** is a web application I developed that allows school admins to manage student marks across different subjects in an organized and user-friendly way. The app is designed for small to medium-sized schools that need a simple solution for tracking grades and academic performance.

> **Note:** Grades was my graduation project for Harvard University's CS50's Introduction to Computer Science, developed entirely from concept to implementation.

## Key Features

- Manage schools, subjects, and students across multiple academic years and semesters
- Comprehensive tracking of grades, percentages, and class rankings for each student
- Dual interface system: separate Admin and Student portals with independent login credentials
- Responsive Bootstrap-based interface that works seamlessly across different screen sizes

## Admin Features

- **School Management:**
    - Create new schools or join existing ones using a unique symbol and password for admin collaboration.
    - Configure school settings including name, number of years, and semesters per year.
- **Subject Management:** 
    - Define subjects with details such as title, code, final mark, and year-semester combination.
    - Easily modify or delete subjects as needed.
- **Student Management:**
    - Add and manage student information including name, code, current year-semester, and secure login credentials (username/password).
- **Academic Tracking:**
    - Automatically calculates and displays total marks, percentages, grades, and class rankings for each student.
- **Flexible Modifications:**
    - Make adjustments to account settings, school configurations, subject details, and student data at any time.

## Student Features

- **Individual Access:**
    - Students log in using their unique credentials (username/password) to view their marks
- **Comprehensive View:**
    - Detailed breakdown of marks by subject, year-semester information, and overall academic performance including class rank

## Screenshots

{{< gallery match="screenshots/*" sortOrder="acs" rowHeight="150" margins="5" thumbnailResizeOptions="600x600 q90 Lanczos" showExif=false previewType="blur" embedPreview=true loadJQuery=true >}}

## Walkthrough Video

{{< youtube "qk_kFFU9T7c" >}}

## Technologies Used

I built Grades using the following technologies:

- **Flask (Python):** Backend framework for server logic, authentication, and session management
- **SQLite:** Lightweight database for storing schools, subjects, students, and grades data
- **HTML, CSS, Bootstrap:** Frontend design with responsive layout
- **Jinja:** Templating engine for dynamic page generation

## Development Background

Grades was one of the earliest web applications I ever built. I conceptualized and designed it from scratch as my final project for Harvard University's CS50's Introduction to Computer Science. The entire development process took approximately three weeks from initial concept to the current stage.

View my CS50 certificate [here](https://certificates.cs50.io/f6fe2bd3-3279-4831-8781-1c8feeb640e4).

## Project Links

View the live demo at [gradesapp.azurewebsites.net](https://gradesapp.azurewebsites.net/)
