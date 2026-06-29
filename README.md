# 🌐 Portfolio Website (Django)

> A personal portfolio website built with Python and Django showcasing all internship projects, skills, and contact information.

---

## 👤 Intern Details

| Field            | Details                     |
|------------------|-----------------------------|
| **Intern ID**    | CITS5322                    |
| **Full Name**    | PREETHI S                   |
| **No. of Weeks** | 4 WEEKS                     |
| **Project Name** | Portfolio Website (Django)  |

---

## 📌 Project Scope

This project is a personal portfolio website built using Python and Django.
The website displays the intern's name, skills, all 4 internship projects,
and contact information in a clean dark-themed single-page layout.

The project covers:
- Setting up a Django project and app from scratch
- Creating URL routing using Django's URL dispatcher
- Building HTML templates using Django's template engine
- Using template inheritance with base.html and block content
- Serving a multi-section single-page website using Django views
- Styling the website using inline CSS with a dark theme

---

## ✨ Features

- 🏠 **Home Section** — Name, title, and intro with a call-to-action button
- 👤 **About Section** — Personal introduction and skills displayed as tags
- 💼 **Projects Section** — All  projects displayed as cards
- 📬 **Contact Section** — Email and location details
- 🧭 **Sticky Navbar** — Navigation links to all sections
- 🎨 **Dark Theme** — Clean modern dark UI throughout

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python | Core programming language |
| Django  | Web framework |
| HTML | Page structure and content |
| CSS | Styling and layout |
| Django Templates | Dynamic page rendering |

---

## 🖥️ Website Sections

| Section | URL | Description |
|---------|-----|-------------|
| Home | `/#home` | Name, title, intro |
| About | `/#about` | Skills and introduction |
| Projects | `/#projects` | All  projects |
| Contact | `/#contact` | Email and location |

---


## 📁 Project Structure

```
Portfolio-Website/
│
└── portfolio/                  # Django project root
    ├── main/                   # Main Django app
    │   ├── templates/
    │   │   └── main/
    │   │       ├── base.html   # Base template with navbar and footer
    │   │       └── home.html   # Main portfolio page
    │   ├── views.py            # View functions for each page
    │   ├── urls.py             # URL routes for main app
    │   ├── models.py           # Database models (unused)
    │   ├── admin.py            # Admin config (unused)
    │   └── apps.py             # App configuration
    ├── portfolio/              # Django project settings
    │   ├── settings.py         # Project settings
    │   ├── urls.py             # Root URL configuration
    │   ├── wsgi.py             # WSGI configuration
    │   └── asgi.py             # ASGI configuration
    ├── manage.py               # Django management tool
    └── README.md               # Project documentation
```

---

## 📖 Documentation

### How the Code Works

#### 1. Django Project Setup
The project was created using `django-admin startproject portfolio` and
the main app was created using `python manage.py startapp main`.
The `main` app was registered in `settings.py` under `INSTALLED_APPS`.

#### 2. URL Routing
`portfolio/urls.py` includes the main app's URLs using `include('main.urls')`.
`main/urls.py` maps each URL path to a view function.

#### 3. Views (views.py)
Each function in `views.py` renders an HTML template and returns it as a response.
All pages point to `main/home.html` since the website is a single page.

#### 4. Template Inheritance
`base.html` contains the navbar, footer, and common HTML structure.
`home.html` extends `base.html` using `{% extends 'main/base.html' %}` and
fills in the content using `{% block content %}`.

#### 5. Single Page Design
All 4 sections (Home, About, Projects, Contact) are in one `home.html` file.
Navbar links use anchor tags (`#home`, `#about`) to scroll to each section.

### Django Concepts Used

| Concept | Where Used |
|---------|------------|
| `startproject` | Create Django project |
| `startapp` | Create main app |
| `urls.py` | URL routing |
| `views.py` | Page rendering functions |
| `render()` | Return HTML response |
| `{% extends %}` | Template inheritance |
| `{% block content %}` | Template blocks |
| `INSTALLED_APPS` | Register main app |
| `include()` | Connect app URLs |

---

## 💼 Projects Showcased

| # | Project | Tech |
|---|---------|------|
| 1 | 🗂️ Automated File Organizer | Python, Tkinter, JSON |
| 2 | 🌤️ Weather App | Python, requests, Open-Meteo API |
| 3 | 💰 Expense Tracker | Python, Tkinter, CSV, JSON |
| 4 | 🌐 Portfolio Website | Python, Django, HTML, CSS |

---

## 📚 Concepts Learned

- Setting up and running a Django project
- URL routing and view functions
- Django template engine and template inheritance
- Building responsive single-page websites
- Serving web pages using Python
- Project structure in Django

---
