# 📝 Django Blog Application

A full-featured blog application built using **Python**, **Django**, and **MySQL**, supporting user authentication, role-based permissions, content publishing, and post management.

---

## 🚀 Features

- 👥 User Registration and Login with Secure Authentication
- 🔐 Password Reset via Email
- 🧑‍💻 Role-Based Access Control (Readers, Authors, Editors)
- ✍️ Create, Edit, Delete, and Publish Blog Posts
- 🖼️ Upload Images to Posts with Default Image Support
- 📄 Post Detail View with Related Posts
- 📑 About Page with Editable Content
- 📬 Contact Form with Email Logging
- 🧭 Pagination for Posts
- 🧹 Clean and Modular Code Structure

---

## 🔧 Tech Stack

- **Backend:** Python, Django
- **Frontend:** HTML, CSS, JavaScript
- **Database:** MySQL
- **Authentication & Permissions:** Django Auth System
- **Email Backend:** Django SMTP (for password reset)
- **Version Control:** Git, GitHub

---

## 📁 Project Structure

blog_project/
├── blog/ # Django app
│ ├── models.py # Models: Post, Category, AboutUs
│ ├── views.py # All view logic
│ ├── forms.py # Contact, Register, Login, Post forms
│ ├── urls.py # URL routing
│ └── templates/ # HTML templates
├── static/ # Static files (CSS, JS, images)
├── media/ # Uploaded media files
├── manage.py
├── README.md


## Configuring MySql in settings.py

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'your_db_name',
        'USER': 'your_mysql_user',
        'PASSWORD': 'your_mysql_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}


## Apply Migrations

python manage.py makemigrations
python manage.py migrate


## Create a Superuser

python manage.py createsuperuser

## Run the Development Server

python manage.py runserver

## Email Configuration for password reset

EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
EMAIL_HOST = 'smtp.yourprovider.com'
EMAIL_PORT = 587
EMAIL_USE_TLS = True
EMAIL_HOST_USER = 'your_email@example.com'
EMAIL_HOST_PASSWORD = 'your_password'
DEFAULT_FROM_EMAIL = EMAIL_HOST_USER



