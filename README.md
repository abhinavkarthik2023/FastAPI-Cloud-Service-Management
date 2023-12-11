# Cloud-Service-Access-Management-System

This project is a FastAPI-based cloud subscription service, integrating SQLAlchemy for database management. It allows for the creation, modification, and deletion of subscription plans, permissions, and user subscriptions. It also includes API usage tracking and access control based on user subscriptions.

# Project Team Members - Group Project 16


Venkata Abhinav Karthik Pulikonda (Cwid -885210294)

Sai Satya Jagannadh Doddipatla (Cwid - 885177436)

Rakesh Puppala (Cwid - )

Piyush Jagtap (Cwid - )



# Drive Link For the Project Demonstration and Screenshots -

## https://drive.google.com/drive/folders/1D9gzEzlfdrF4OA089lipezQhRt42p91e?usp=sharing](https://drive.google.com/drive/folders/1glbYEe3w4sCLLGcXtVHQt_KbYG5L9AXw?usp=sharing


# Project Description

This project involves developing a backend system for managing access to cloud services based on user subscriptions. The primary users of the system are Customers who access cloud services and Admins who manage subscription plans and permissions. The system will regulate access to various cloud APIs based on the subscription plan purchased by the customer. If a customer exceeds the maximum limit of a service as defined in their plan, access to that specific service will be temporarily restricted.

# Objectives

● To develop a backend system that dynamically manages access to cloud services based on user subscriptions.

● To implement a role-based access control (RBAC) system where the admin can modify user permissions and subscription plans.

● To simulate cloud service usage and enforce limits based on subscription plans.



# Features

## Subscription Plan Management: Create, view, modify, or delete subscription plans.
## Permission Management: Modify or delete permissions.
## User Subscription Handling: Subscribe users to plans and view their subscriptions.
## Access Control: Check users' access permissions to different API endpoints.
## Usage Tracking: Track and manage users' API usage.


# Requirements

● FastAPI

● SQLAlchemy

● MySQL Connector

● Python 3.6+


# Installation

Install the required packages using pip:

## pip install fastapi sqlalchemy mysql-connector-python


# Database Configuration

MySQL database is required.

Configure the DATABASE_URL in the code to point to your MySQL instance.

# Models

## Database Models

 Plan: Represents subscription plans.

 Permission: Represents permissions.

 Subscription: Links users to their subscription plans.

 User: User data.

 Usage: Tracks API usage by users.


## Pydantic Models

PlanCreate, PermissionCreate, SubscriptionCreate, etc., are Pydantic models for request validation.

# Endpoints

 Subscription Plans : POST /plans/{token}, GET /plans/{plan_id}, PUT /plans/{plan_id}/{token}, DELETE /plans/{plan_id}/{token}

 Permissions : PUT /permissions/{permission_id}/{user_id}, DELETE /permissions/{permission_id}/{user_id}

 User Subscriptions : POST /subscriptions/{user_id}, GET /subscriptions/{user_id}

 Access Control : GET /access/{user_id}/{api_request}

 Usage Tracking : GET /usage/{type}/{user_id} where {type} can be a, b, or c for different API endpoint types.


# Running the Application

To run the server, execute:

## uvicorn main:app --reload

* Replace main with the name of your Python file.

Notes

* Ensure your MySQL service is running and accessible.

* The application is designed for learning and development purposes and may require modifications for production use.


  
