# django_blog_challenge

Challenge Overview

    Help future developers understand this Django blog application by adding comprehensive code comments and documentation! This challenge focuses on code readability, documentation best practices, and Django/Python conventions.

Challenge Objectives:

    1. Code Documentation

        Add detailed docstrings to all classes and functions explaining what they do and why they are needed.

    2. Add Comments to the Blog Project

        Please use the current code base and add comments to the blog entries. For bonus credit, make the comments reviewable on the django admin and allowed to be removed at any point. 

Django Blog

    A simple, modern blog application built with Django 5.0 and Bootstrap 5. This project includes user authentication, blog post creation/management, and a responsive design.

Features

    User authentication (login/logout)
    Blog post management (create, read, update, delete)
    Responsive design using Bootstrap 5
    Image upload support
    Comment system
    Admin interface
    Slug-based URLs
    Pagination

Prerequisites

    Python 3.8 or higher
    pip package manager
    Virtual environment (recommended)

Installation

    Clone the repository:

    git clone <repository-url>
    cd django-blog

Create and activate a virtual environment:

    python -m venv env
    source env/bin/activate  # On Windows: .\env\Scripts\activate

Install required packages:

    pip install -r requirements.txt

Configure environment variables:

    # Create .env file in the project root
    SECRET_KEY=your-secret-key
    DEBUG=True
    ALLOWED_HOSTS=localhost,127.0.0.1

Run migrations:

    python manage.py makemigrations
    python manage.py migrate

Create a superuser (this will be the user you use to access the admin and/or post blogs directly on the frontend):

    python manage.py createsuperuser

Start the development server:

    python manage.py runserver
    The application will be available at http://127.0.0.1:8000

Project Structure

    django-blog/
    ├── blog_project/          # Main project directory
    │   ├── settings.py        # Project settings
    │   └── urls.py           # Main URL configuration
    ├── blog/                  # Blog application
    │   ├── models.py         # Database models
    │   ├── views.py          # View functions
    │   ├── urls.py           # Blog URL configuration
    │   └── forms.py          # Forms
    ├── templates/            # HTML templates
    │   ├── base.html
    │   └── blog/
    ├── static/              # Static files
    ├── media/              # User-uploaded files
    ├── requirements.txt    # Project dependencies
    └── manage.py          # Django management script

Built With:

    Django - Web framework
    Bootstrap - Frontend framework
    Pillow - Image processing
    python-dotenv - Environment management

