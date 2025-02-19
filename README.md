# Django Authentication & User Management System

## Overview

**User Authentication and Management System** built with **Django**. This project provides robust features for user management, including **user registration**, **login/logout**, **profile management**, and **role-based access control** using groups. It uses **Django Signals** for automatically assigning new users to a **default group** upon registration. The user interface is built using **HTML**, **CSS**, and **Bootstrap 5** to ensure a responsive and clean design.

---

## Key Features

- **User Registration**: New users can sign up with their email and password.
- **User Authentication**: Secure login and logout functionality using Django's built-in authentication system.
- **Role-based Access Control**: Automatically assigns users to a **default** group upon registration and allows admins to manage different roles (e.g., admin, moderator, user).
- **Admin Panel**: The Django admin panel allows admins to manage users, groups, roles, and permissions.
- **Responsive UI**: Built using **HTML**, **CSS**, and **Bootstrap 5** to provide a modern, mobile-friendly design.
- **Django Signals**: Automatically assigns new users to the "default" group through Django's signals when they register.

---

## Tools & Technologies Used

- **Django**: A high-level Python web framework for building scalable and secure web applications.
- **PostgreSQL**: A powerful relational database management system to store user data securely.
- **Django Signals**: For triggering actions automatically (e.g., adding new users to a default group after registration).
- **HTML, CSS, Bootstrap 5**: For creating a modern, responsive, and user-friendly front-end design.
- **Django Admin**: For managing users, groups, and roles via the Django admin interface.

---

## Setup & Installation

Follow the steps below to get the project up and running locally:

1. **Clone the repository**:
2. 
   git clone 
   cd django-authentication-user-management

3. **Set up a virtual environment**:

    python -m venv venv
    source venv/bin/activate  # For Linux/Mac
    venv\Scripts\activate     # For Windows
   
5. **Install dependencies**:

     pip install -r requirements.txt

6. **Set up the database**:

     python manage.py migrate

7. **Create a superuser for the admin panel**:

     python manage.py createsuperuser

8. **Run the development server**:

     python manage.py runserver


Access the Admin Panel:
Visit the Django admin at http://127.0.0.1:8000/admin/ to manage users, groups, and permissions.

Features in Detail
1. User Registration
Users can register by providing an email and password. After successful registration, users are automatically added to the default group through a Django signal.

2. User Authentication
Secure login and logout functionality is provided using Django’s built-in authentication system. Sessions are handled automatically for each user.

3. Profile Management
Users can update and manage their personal details (e.g., name, email). This feature allows users to keep their profile information up-to-date.

4. Role-based Access Control
Upon registration, users are assigned to the default group. Admin users can manage additional groups (e.g., admin, moderator) and assign specific permissions to each group.

5. Django Admin Panel
The Django admin interface allows easy management of users, groups, and roles. Admin users can assign, update, or remove users from different groups and configure permissions.

6. Responsive User Interface
The user interface is designed to be responsive using Bootstrap 5, ensuring the system works seamlessly on both desktop and mobile devices.

9. Django Signals
Django’s built-in signals are used to trigger automatic actions, such as adding new users to the default group when they register.

Requirements:

Python 3.x
Django >=4.0
PostgreSQL (for production database)



Install Dependencies:
pip install -r requirements.txt


