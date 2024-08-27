Twitter Clone (now "X")

Overview:
This Twitter Clone project is an extension of an existing web application intended to provide practice in understanding, fixing, and enhancing a codebase. The application simulates key features of Twitter, such as user authentication, posting messages (warbles), following other users, and liking posts. The project focuses on reading and understanding the existing code, fixing bugs, writing tests, and implementing new features.


Features:
User authentication (login, logout, registration)
User profile with bio, location, and header image
Posting and deleting messages (warbles)
Following and unfollowing other users
Liking and unliking warbles
Custom user profile edit functionality
Display of the last 100 warbles from followed users on the homepage

Technologies used:
Python: Core programming language for backend logic
Flask: Web framework used to handle routing and server-side logic
SQLAlchemy: ORM for database interactions
WTForms: Form handling and validation
Jinja2: Templating engine for rendering HTML
PostgreSQL: Database for storing user data and warbles
HTML/CSS: Frontend structure and styling

Setup:

Prerequisites
Python 3.x installed on your system
PostgreSQL installed and running

Clone the Repository:
git clone https://github.com/manroopSandhu/30.twitterclone
cd twitterClone

Create and Activate a Virtual Environment:
python3 -m venv venv
source venv/bin/activate

Install Dependencies:
pip install -r requirements.txt
Note: If using Python 3.8, remove psycopg2-binary from requirements.txt and install it manually using pip install psycopg2-binary.

Set Up the Database:
createdb warbler
python seed.py

Run the Application:
flask run

Project Structure:
twitter-clone/
│
├── app.py               # The main Flask application
├── models.py            # Database models
├── forms.py             # WTForms for handling form data
├── seed.py              # Script for seeding the database with initial data
├── static/
│   └── styles.css       # CSS file for styling
├── templates/
│   ├── base.html        # Base template for extending other templates
│   ├── home.html        # Homepage template
│   ├── profile.html     # User profile page template
│   ├── ...              # Other HTML templates
├── test/
│   ├── test_user_model.py   # Unit tests for User model
│   ├── test_user_views.py   # Unit tests for User views
│   ├── test_message_model.py  # Unit tests for Message model
│   ├── test_message_views.py  # Unit tests for Message views
├── requirements.txt     # List of dependencies
└── README.md            # This file













