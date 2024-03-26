# GPA Calculator

A Django web application that allows users to calculate their GPA by entering subjects, their respective grades, and credit hours. This app includes user authentication, allowing users to register, login, and manage their subject entries for GPA calculation. It also features a PDF generation for the GPA report.

## Features

- **User Authentication**: Register and login functionality to keep your subject entries private and secure.
- **Subject Management**: Add, edit, and delete subject entries including their name, grade, and credit hours.
- **GPA Calculation**: Automatically calculates your GPA based on the subjects and grades entered.
- **PDF Generation**: Generate a PDF version of your GPA report for printing or saving.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.8 or above installed on your system.
- Django 3.x installed in your Python environment.

## Installation and Setup

1. Clone the repository:
```bash
git clone https://github.com/soheill2001/GPA-Calculator.git
cd GPA-Calculator
```
2. Set up a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

3. Install the dependencies:
```bash
pip install -r requirements.txt
```

4. Apply migrations to create the database schema:
```bash
python manage.py makemigrations
python manage.py migrate
```

5. Create a superuser account (optional but recommended for accessing the Django admin site):
```bash
python manage.py createsuperuser
```

6.Run the development server:
```bash
python manage.py runserver
```
Your app should now be running on http://127.0.0.1:8000.

## Usage
After starting the server, you can access the following functionalities:

- Visit http://127.0.0.1:8000/register to create a new user account.
- Log in with your credentials athttp://127.0.0.1:8000/login.
Once logged in, use the form to add your subjects along with their grades and credit hours.
- Edit or delete subjects using the corresponding buttons next to each subject entry.
- Your GPA is calculated and displayed at the bottom of the page.
- To generate a PDF report of your GPA, click the "Generate Result" button.