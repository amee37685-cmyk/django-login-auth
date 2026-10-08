# Django Login and Authentication

A simple Django web application with user login, logout and a protected home page.

## Features
- User login with username and password
- Logout functionality
- Home page accessible only to logged-in users (anonymous users are redirected to the login page)
- Error message shown on wrong username or password
- Bootstrap 5 styled login page with show/hide password toggle
- Django admin panel for user management

## Technologies Used
- Python 3
- Django
- SQLite
- HTML, CSS, JavaScript
- Bootstrap 5

## Python Concepts Used
- Functions and view functions
- Conditional statements (`if/else`)
- HTTP request handling (GET and POST)
- Django messages framework
- Imports and modules

## Database
The project uses the default SQLite database (`db.sqlite3`). User accounts are stored using Django's built-in `User` model. The database file is not included in this repository.

## Project Structure
```
Userproject/
├── home/            # Main app (views, urls)
├── templates/       # index.html, login.html
├── static/          # Static files
├── Userproject/     # Project settings and urls
└── manage.py
```

## Installation
```
git clone https://github.com/amee37685-cmyk/django-login-auth.git
cd django-login-auth
pip install django
python manage.py migrate
python manage.py createsuperuser
```

## Run the Project
```
python manage.py runserver
```
Then open `http://127.0.0.1:8000/login` in your browser and sign in with the superuser you created.

## Future Improvements
- User registration (sign up) page
- Forgot password / password reset by email
- "Remember me" functionality
- Google and Facebook login
- Unit tests