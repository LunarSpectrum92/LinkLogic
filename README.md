# APLIKACJA INTERNETOWA FIRMY E-COMMERCE

Project Overview:
	This project is a web application designed for an e-commerce company specializing in IT services. System allow to manage tasks and assign them to specific employees. It also provides booking system and view of task proggress for users.

## System roles
1.client
2.employee
3.admin

## Table of Contents
1. [Features](#features)
2. [Technologies](#technologies)
3. [Database Design and Structure](#database-design-and-structure)
4. [ERD](#ERD)
5. [Screenshots](#screenshots)


### 1. Authentication & Registration
* **User Registration:** New clients can create accounts.
* **Multi-Role Login:** Unified login system for all actors: **Admin**, **Client**, and **Employee**.

### 2. Role-Based Access Control (RBAC)
Specific modules are accessible based on the user's role:

#### Client
* **Booking Creation:** Can place new service reservations.
* **Tracking:** Can view and monitor their own bookings.

#### Admin
* **User Management:**
    * Manage user permissions and roles.
    * Delete user accounts.
* **Booking Management:**
    * Update booking statuses.
    * Assign tasks to specific employees.
    * Delete booking records.

#### Employee
* **Task Overview:** View a list of tasks assigned by the Admin.
* **Task Completion:** Change task status to "Completed" (records are then removed from the active list).

### 3. Account Information
* **Profile Access:** Every user can view their personal data within the system.

### 4. Logout
* **Session Termination:** Users can securely log out of their accounts.

### 5. Session & Access Management
* **Session Handling:** Each successful login initializes a unique user session.
* **Route Protection:** Users attempting to access restricted pages without proper permissions are automatically redirected to the homepage.


## Technologies

- HTML
- CSS
- JavaScript
- PHP
- NGINX
- PostgresSQL
- Docker


## Database Design and Structure

	-users: user data
		-name
		-surname
		-email
		-password
		-role
	-user_details: user data
		-phonenumber
		-street
		-city
	-orders: zamowienia
		-opis
		-data
		-status
	-service: usługi
		-ServiceName
		-price
	-employee_orders
		-user_id
		-order_d

![ERD](zdjecia/erd.png)


## UML
![UML](zdjecia/uml.png "UML")

## Screenshots
zdjecia poszczególnych części projektu

![Homepage](zdjecia/main.png "Homepage")
![Login Screen](zdjecia/login.png "Login Screen")
![Admin User Profile](zdjecia/adminDashboard.png "Admin User Profile")
![users](zdjecia/użytkownicy.png "users")
![reservations](zdjecia/rezerwacje.png "reservations")
![contact](zdjecia/kontakt.png "contact")
![offer](zdjecia/oferta.png "offer")
![register](zdjecia/rejestracja.png "register")
![rezerwation](zdjecia/rezerwacja.png "rezervation")

		