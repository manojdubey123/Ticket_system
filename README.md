# Django Ticketing System

A Django-based ticketing system for managing tasks with user authentication, ticket creation, assignment, activity tracking, and notifications.

## Features

- **User Authentication**: Login and logout functionality for secure access.
- **Ticket Management**: Create, assign, view, and track tickets with priority and status options.
- **Activity Tracking**: Users can update ticket status and add comments for detailed tracking.
- **Admin Capabilities**: Admins can manage all tickets, including assigning users.
- **Notifications**: Email notifications for ticket assignments and updates.

## Prerequisites

- **Python 3.x**
- **Django 3.x or later**
- **MySQL**

## Setup Instructions

### Step 1: Create and Activate a Virtual Environment

- python -m venv env
- source env/bin/activate  # On Windows use `env\Scripts\activate`

### Install Dependencies
-pip install -r requirements.txt

###  MySQL Database Setup

- Install MySQL (if not already installed).
- Create a Database: Open your MySQL shell and create a new database.

- In settings file we 
- DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'ticketing_db',
        'USER': 'ticket_user',
        'PASSWORD': 'your_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}

###  For Notification Setup

- For Notification you need to set up this 

SECRET_KEY='your_django_secret_key'
DEBUG=True
EMAIL_HOST='smtp.your_email_service.com'
EMAIL_PORT=587
EMAIL_HOST_USER='your_email@example.com'
EMAIL_HOST_PASSWORD='your_email_password'
EMAIL_USE_TLS=True

###  Run Migrations

- python manage.py makemigrations,
- python manage.py migrate

### For Create Superuser
- python manage.py createsuperuser


### For running the server
- python manage.py runserver


### Clone the Repository



```bash
git clone <repository-url>
cd django-ticketing-system


