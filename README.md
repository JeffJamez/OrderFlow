# OrderFlow

A production-ready online ordering system built with Django that demonstrates secure authentication, scalable architecture, and clean separation of concerns. Designed to handle real-world e-commerce workflows including product management, cart operations, and order processing.

## Value Proposition

OrderFlow solves the core challenge of building a secure, maintainable ordering platform from scratch. It implements industry best practices including password hashing, CSRF protection, session management, and admin controls—making it an ideal reference for recruiters evaluating full-stack Django proficiency.

## Core Features

- Secure user authentication with Django's built-in auth system and PBKDF2 password hashing
- Product catalog with image support, categorization, and detailed views
- Shopping cart with quantity management and real-time price calculation
- Order workflow with status tracking and admin oversight
- Django Admin integration for efficient product and order management
- Static and media file handling configured for development and production readiness
- Form validation and error handling with user-friendly feedback

## Technical Architecture

Backend: Python 3.x, Django 3.x, Django REST Framework (if applicable)
Database: SQLite (development), easily configurable for PostgreSQL/MySQL
Frontend: HTML5, CSS3, JavaScript with Django templating
Security: CSRF tokens, secure session cookies, input sanitization
Deployment: WSGI-ready, environment variable configuration via python-decouple or dotenv

## Project Structure

OrderFlow/
├── accounts/           # Authentication, user profiles, permissions
├── orders/             # Cart logic, order models, checkout workflow
├── products/           # Product models, views, admin configuration
├── static/             # CSS, JavaScript, and image assets
├── media/              # User-uploaded product images
├── templates/          # Reusable Django HTML templates
├── manage.py           # Django CLI entry point
├── requirements.txt    # Reproducible dependency management
└── README.md           # Project documentation

## Setup Instructions

1. Clone the repository
   git clone https://github.com/JeffJamez/Online-Ordering-App.git
   cd Online-Ordering-App

2. Create and activate a virtual environment
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate

3. Install dependencies
   pip install -r requirements.txt

4. Apply database migrations
   python manage.py migrate

5. Create an admin user
   python manage.py createsuperuser

6. Run the development server
   python manage.py runserver

7. Access the application at http://localhost:8000

## Key Technical Decisions

- Chose Django's class-based views for reusability and maintainability
- Implemented custom permission classes to control access to order management
- Used Django's messages framework for non-intrusive user feedback
- Structured templates with inheritance to reduce duplication and improve consistency
- Configured MEDIA_ROOT and STATIC_ROOT for straightforward production deployment

## Testing and Quality

- Form validation tested with Django's test client
- Authentication flows verified with unit tests
- Code formatted with Black and linted with Flake8 (optional but recommended)
- Clear commit history demonstrating iterative development and problem-solving

## Why This Project Stands Out to Recruiters

- Demonstrates mastery of Django's ORM, authentication system, and admin interface
- Shows understanding of security fundamentals critical for production applications
- Clean, documented code that follows PEP 8 and Django best practices
- Modular design that scales—easy to extend with payment integration, email notifications, or API endpoints
- Solves a real business problem with a polished, user-focused interface

## Contributing

1. Fork the repository
2. Create a feature branch: git checkout -b feature/YourFeature
3. Commit changes: git commit -m 'Add YourFeature'
4. Push to branch: git push origin feature/YourFeature
5. Submit a pull request with a clear description of changes

## License

MIT License. See LICENSE file for details.

## Author

Jeff James
