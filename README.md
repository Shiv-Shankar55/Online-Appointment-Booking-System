# 🩺 Online Doctor Appointment Booking System

A web-based **Online Doctor Appointment Booking System** that allows users to register, log in, view available doctors, select appointment date and time slots, book appointments, and manage their existing appointments.

The system is designed to make doctor appointment booking easier, faster, and more convenient while storing appointment information in a PostgreSQL database.

---

## 📌 Project Overview

The **Online Doctor Appointment Booking System** is a web application developed using **JSP, JDBC, HTML, CSS, JavaScript, and PostgreSQL**.

Users can access the system online, register for an account, log in, view available doctors, choose a suitable date and time, and confirm their appointment. Appointment details are stored in the database for easy management.

---

## ✨ Features

- 🏠 Home page with navigation and project information
- 📝 User registration
- 🔐 User login and authentication
- 👨‍⚕️ View available doctors
- 🩺 View doctor specialization and consultation fee
- 📅 Select appointment date
- ⏰ Select appointment time
- ✅ Confirm doctor appointments
- 📋 View booked appointments
- ❌ Cancel/Delete appointments
- 🚪 User logout using session management
- ✔️ Registration and login form validation

---

## 🛠️ Technologies Used

| Category | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | JSP, JDBC |
| Database | PostgreSQL |
| Server | Apache Tomcat |
| IDE | Eclipse |

These are the technologies and development tools specified in the project presentation.

---

## 📂 Project Modules

The system consists of the following major modules:

1. **Home Page**
2. **User Registration**
3. **User Login**
4. **Doctor Selection**
5. **Appointment Booking**
6. **Appointment View**
7. **Delete / Cancel Appointment**
8. **User Logout**



---

## 🗄️ Database Design

The application uses **PostgreSQL** as its database.

### Users Table

| Column | Data Type |
|---|---|
| id | INT |
| name | VARCHAR |
| email | VARCHAR |
| password | VARCHAR |

### Doctors Table

| Column | Data Type |
|---|---|
| id | INT |
| doc_name | VARCHAR |
| specialization | VARCHAR |
| fee | INT |
| image | VARCHAR |

### Appointments Table

| Column | Data Type |
|---|---|
| id | INT |
| user_name | VARCHAR |
| doctor_name | VARCHAR |
| specialization | VARCHAR |
| appointment_date | DATE |
| appointment_time | VARCHAR |



---

## 🔐 Validation

The project includes validation for both registration and login.

### Registration Validation

- All required fields must be filled.
- Password must contain at least **8 characters**.
- Password must include:
  - One uppercase letter
  - One lowercase letter
  - One number
  - One special character
- Password and confirm password must match.

The registration validation is implemented in `register.jsp`.

### Login Validation

- Email and password fields are checked.
- Users can log in only after successfully registering.

The login validation is implemented in `login.jsp`.

---

## 🎨 CSS Structure

Different CSS files are used to style different sections of the application:

```text
home.css
login.css
register.css
appointment.css
myAppointment.css
nav.css
footer.css
doctor.css
```

### CSS Responsibilities

- `home.css` — Overall page layout and common styling
- `login.css` — Login page, input fields, and buttons
- `register.css` — Registration form
- `appointment.css` — Appointment booking page
- `myAppointment.css` — Booked appointment table and details
- `nav.css` — Navigation bar
- `footer.css` — Footer
- `doctor.css` — Doctor cards, profiles, and doctor list



---

## 🖥️ Application Pages

### 🏠 Home Page

**File:** `home.jsp`

Includes:

- Navigation bar
- Home, About, and Contact options
- Login/Logout button
- Hero section
- Book Now button
- Find Doctors
- Manage Appointments
- Reminders



---

### 📝 Registration Page

**File:** `registration.jsp`

Users can provide:

- Full Name
- Email
- Password
- Confirm Password

The page also provides a link to the Login page.

---

### 🔐 Login Page

**File:** `login.jsp`

Users can log in using:

- Email Address
- Password

The page also contains:

- Login button
- Register Now link
- Back to Home option



---

### 👨‍⚕️ Doctors Page

**File:** `doctor.jsp`

Displays:

- Available doctors
- Doctor image
- Doctor name
- Specialization
- Consultation fee
- Book Appointment button



---

### 📅 Book Appointment Page

**File:** `appointment.jsp`

Users can:

- Select appointment date
- Select appointment time
- Confirm the booking



---

### 📋 My Appointments

**File:** `myAppointment.jsp`

Displays the user's booked appointments, including:

- Doctor name
- Specialization
- Appointment date
- Appointment time
- Delete/Cancel option



---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/online-doctor-appointment-booking-system.git
```

### 2. Open the Project

Open the project in **Eclipse**.

### 3. Configure PostgreSQL

Create a PostgreSQL database and configure the database connection used by the application.

Example:

```text
Database: appointment_booking
Host: localhost
Port: 5432
Username: your_username
Password: your_password
```

> ⚠️ Do not upload your actual database password or other sensitive credentials to GitHub.

### 4. Configure Apache Tomcat

Add **Apache Tomcat** to Eclipse and configure the project to run on the Tomcat server.

### 5. Run the Application

Start the Tomcat server and open the application in your browser.

```text
http://localhost:8080/YourProjectName/
```

---

## 🔄 Application Workflow

```text
User
  │
  ▼
Home Page
  │
  ▼
Register
  │
  ▼
Login
  │
  ▼
View Doctors
  │
  ▼
Select Doctor
  │
  ▼
Select Date & Time
  │
  ▼
Confirm Appointment
  │
  ▼
My Appointments
  │
  ├── View Appointment
  │
  └── Cancel Appointment
```

---

## 🚀 Future Enhancements

The project can be further improved by adding:

- 💳 Online payment integration
- 📱 SMS notifications
- 📧 Email appointment alerts
- 👨‍💼 Admin panel
- 📱 Mobile application support

These enhancements are also identified in the project's presentation.

---

## 👨‍💻 Team Members

### Sibasankar Panda

**Branch:** CSE  
**Section:** D1  
**Group:** 12  
**Lab Roll No:** 3

**Contribution:**
- Developed Home Page
- Developed Login Page
- Developed Registration Page
- Frontend design
- Backend functionality using JSP

### Ankit Kumar

**Branch:** CSE  
**Section:** D1  
**Group:** 12  
**Lab Roll No:** 31

**Contribution:**
- Developed Doctor Appointment Booking Page
- Developed Manage Appointment Page
- Frontend design
- Backend functionality using JSP



---

## 📚 Academic Project

**Course:** Internet & Web Technology (IWT)  
**Program:** B.Tech – Computer Science and Engineering  
**Semester:** 4th Semester

---

## 📄 License

This project was developed as an academic project for educational purposes.