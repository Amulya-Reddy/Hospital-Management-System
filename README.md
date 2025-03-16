# Hospital Management System

## Overview
The **Hospital Management System** is a web-based application built using **Flask** and **MySQL** to efficiently manage hospital operations such as patient records, doctor schedules, and appointments. It provides an intuitive interface for administrators, doctors, and patients to interact seamlessly.

## Features
- **Patient Management**: Add, update, and delete patient records.
- **Doctor Management**: Maintain doctor profiles and schedules.
- **Appointment Booking**: Patients can book and track appointments.
- **User Authentication**: Secure login system for different user roles (Admin, Doctor, Patient).
- **Billing System**: Generate and manage hospital billing.
- **Dashboard & Reports**: Data visualization using **Flask-SQLAlchemy** and **Bootstrap**.

## Technologies Used
- **Backend**: Flask (Python)
- **Frontend**: HTML, CSS, JavaScript, Bootstrap
- **Database**: MySQL (Using Flask-SQLAlchemy)
- **Server**: XAMPP (for local MySQL server)

## Installation
### Prerequisites
- Python (>=3.7)
- MySQL Server (XAMPP recommended)
- Virtual Environment (Optional but recommended)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hospital-management-system.git
   cd hospital-management-system
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # For Mac/Linux
   venv\Scripts\activate  # For Windows
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Configure the database:
   - Start MySQL in XAMPP
   - Create a new database `hospital_db`
   - Update `config.py` with MySQL credentials
   
5. Run database migrations:
   ```bash
   flask db init
   flask db migrate -m "Initial migration"
   flask db upgrade
   ```
6. Start the Flask application:
   ```bash
   flask run
   ```
   The application will be accessible at `http://127.0.0.1:5000`

## Usage
- **Admin**: Can manage doctors, patients, appointments, and billing.
- **Doctors**: Can view their schedules and manage patient records.
- **Patients**: Can book and track appointments.

## Folder Structure
```
Hospital-Management-System/
│── app/
│   ├── static/
│   ├── templates/
│   ├── routes.py
│   ├── models.py
│   ├── forms.py
│── migrations/
│── config.py
│── requirements.txt
│── run.py
│── README.md
```

