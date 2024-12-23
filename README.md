## Airline Booking System
A Django-based airline booking system that enables users to search for available flights, book flights, and manage passenger details. This project exposes a REST API for programmatic access to flight and passenger information, using Django REST Framework.

### Table of Contents
Project Description
Features
Technologies Used
Installation Instructions
Prerequisites
Steps
API Endpoints
Flights
Passengers
Bookings
Usage
For Users
For Developers
Contributing
License
Contact
# Project Description
The Airline Booking System provides a platform to manage flight bookings, passenger details, and flight schedules. It offers the following capabilities:

Browse available flights: Users can search for flights based on their preferences.
Book and manage reservations: Users can book flights and manage their reservations.
Passenger management: Users can add, update, or remove passenger information.
RESTful API: A REST API to integrate flight and passenger data with external systems.
This system is built using Django for the backend and Django REST Framework for the API. It aims to offer a scalable solution for handling flight reservations and customer management.

# Features
Flight Management: Add, update, and delete flights.
Passenger Management: Add, update, and manage passengers.
Booking System: Users can book flights and manage their reservations.
REST API: Exposes flight and passenger functionalities through a comprehensive REST API.
Admin Interface: Built-in Django admin interface for managing flights, passengers, and bookings.
# Technologies Used
This project utilizes the following technologies:

Django – The web framework for building the application.
Django REST Framework – For building the REST API.
SQLite – Lightweight database for development and testing.
Python 3.x – The programming language for developing the system.
Git – Version control system for managing the codebase.
# Installation Instructions
To set up and run the Airline Booking System locally, follow these steps:

Prerequisites
Python 3.x installed on your system.
Git installed on your system.
Virtual environment management tool (e.g., venv).
Steps
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/airline_booking_system.git
cd airline_booking_system
Set up a virtual environment:

On Windows:
bash
Copy code
python -m venv venv
venv\Scripts\activate
On macOS/Linux:
bash
Copy code
python3 -m venv venv
source venv/bin/activate
Install required dependencies: In the project directory, run:

bash
Copy code
pip install -r requirements.txt
Run database migrations: Apply the migrations to set up the database schema:

bash
Copy code
python manage.py migrate
Create a superuser (optional): Create an admin user for accessing the Django admin panel:

bash
Copy code
python manage.py createsuperuser
Start the development server: Run the server:

bash
Copy code
python manage.py runserver
The system will be available at: http://127.0.0.1:8000/

# API Endpoints
The Airline Booking System exposes the following API endpoints:

Flights
GET /api/flights/ – List all available flights.
POST /api/flights/ – Create a new flight.
GET /api/flights/{id}/ – Retrieve details of a specific flight.
PUT /api/flights/{id}/ – Update flight details.
DELETE /api/flights/{id}/ – Delete a specific flight.
Passengers
GET /api/passengers/ – List all passengers.
POST /api/passengers/ – Create a new passenger.
GET /api/passengers/{id}/ – Retrieve details of a specific passenger.
PUT /api/passengers/{id}/ – Update passenger details.
DELETE /api/passengers/{id}/ – Delete a specific passenger.
Bookings
POST /api/bookings/ – Book a flight for a passenger.
GET /api/bookings/{id}/ – View a specific booking.
# Usage
For Users:
Visit http://127.0.0.1:8000/ to browse available flights.
Navigate to the Django admin interface at http://127.0.0.1:8000/admin/ to manage flights, passengers, and bookings (after creating a superuser).
For Developers:
API Access: Use the API endpoints to manage flights, passengers, and bookings programmatically.
Enhancements: Implement additional features, such as notifications, payment integration, or flight search filters.



