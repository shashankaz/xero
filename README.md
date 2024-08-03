# Chirpster

Chirpster is a Twitter-like web application built using Django. Authenticated users can create, update, and delete tweets. The application also includes user authentication and search functionality.

## Features

- User Registration and Authentication
- Create, Edit, and Delete Tweets
- Search Tweets
- Home Page with all the Tweets

## Project Structure

```
xero/
│
├── xero/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── ...
│
├── tweet/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   ├── views.py
│   └── ...
│
├── manage.py
└── ...
```

## Setup Instructions

### Prerequisites

- Python 3.6+
- Django 3.2+
- Virtualenv (optional but recommended)

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/shashankaz/xero.git
   cd xero
   ```

2. **Create and activate a virtual environment:**

   ```bash
   py -m venv .venv
   source .venv\Scripts\activate
   ```

3. **Install the dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Apply migrations:**

   ```bash
   python manage.py migrate
   ```

5. **Create a superuser:**

   ```bash
   python manage.py createsuperuser
   ```

6. **Run the development server:**

   ```bash
   python manage.py runserver
   ```

7. **Visit the application in your web browser:**

   ```
   http://127.0.0.1:8000/
   ```

## URL Configuration

### Main URLs

- Home: `/`
- Admin: `/admin/`
- Tweets: `/tweet/`

### Tweet URLs

- List Tweets: `/tweet/`
- Create Tweet: `/tweet/create/`
- Edit Tweet: `/tweet/<int:tweet_id>/edit/`
- Delete Tweet: `/tweet/<int:tweet_id>/delete/`
- Search: `/tweet/search/`
