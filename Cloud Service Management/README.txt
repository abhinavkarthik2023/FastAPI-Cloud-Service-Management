FastAPI Cloud Subscription Service
===================================

Overview
--------

This FastAPI Cloud Subscription Service is a robust backend system designed to manage cloud-based subscription plans, user subscriptions, permissions, and API access control. It utilizes FastAPI for efficient API development and SQLAlchemy for seamless database interactions, catering to high-performance cloud services environments.

Prerequisites
-------------

- Python 3.6 or higher
- MySQL Server

Installation
------------

1. Clone the repository:

git clone [repository-url]


2. Navigate to the project directory:

cd [project-directory]


3. Install required Python packages:

pip install -r requirements.txt


4. Ensure MySQL Server is installed and running.


Configuration
-------------

1. Update the `DATABASE_URL` in the source code to reflect your MySQL database credentials and server details.

2. Initialize the database by running the provided initialization scripts, if any.

Usage
-----

1. Start the FastAPI server:

uvicorn main:app --reload


2. Access the API endpoints through the provided URL (typically `http://127.0.0.1:8000`).


Features
--------

- **Subscription Plan Management**: Create, read, update, and delete subscription plans.
- **Permission Management**: Modify and delete permissions.
- **User Subscription Handling**: Manage user subscriptions to different plans.
- **Access Control**: Control user access to various API endpoints based on subscription.
- **API Usage Tracking**: Monitor and limit user API usage.

Documentation
-------------

API documentation is automatically generated and can be accessed at `/docs` or `/redoc` endpoints.


Contributing
------------

Project Team Members - Group Project 16

Venkata Abhinav Karthik Pulikonda (Cwid -885210294)

Sai Satya Jagannadh Doddipatla (Cwid - 885177436)

Rakesh Puppala (Cwid - )

Piyush Jagtap (Cwid - )


Acknowledgements
----------------
This project was developed as part of the California State University Fullerton's [CPSC 449/Web-Backend Engineering]. 
Special thanks to Professor Harsh Bodgal and the contributors.




---
End of README.txt



