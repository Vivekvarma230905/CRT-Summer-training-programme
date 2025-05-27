# 🧾 Student Mess Bill Management System

## 📌 Overview

The **Student Mess Bill Management System** is a web-based application designed to automate and simplify the process of mess billing, student attendance tracking, and monthly expense calculation in hostels or educational institutions. It ensures efficient interaction between students and administrators through a secure, responsive interface.

---

## 🎯 Objective

To provide an efficient, transparent, and digital solution for managing student mess expenses and attendance records.

---

## 👥 Users

- **Admin**: Manages student details, monthly expenses, and attendance records.
- **Student**: Views personal mess bill, attendance, and profile.

---

## ✅ Functionalities

- Student Registration and Login  
- Admin Login  
- Monthly Mess Expense Entry  
- Student Attendance Tracking  
- Automatic Expense Calculation  
- Student Dashboard for Expense & Attendance View  
- Secure Authentication  
- Database Integration  
- Responsive UI for Admin & Students  

---

## 🛠️ Project Structure and Files

### 1. 📄 HTML Frontend Files

#### `index.html`
- Landing page with links to Admin and Student login pages.
- Bootstrap-powered responsive layout.

#### `studentlogin.html`
- Login form for students.
- Fields: Student ID, Phone Number.
- Includes JavaScript form validation.

#### `studentregistration.html`
- Registration form for new students.
- Fields: ID, Name, Branch, Phone Number.
- Uses POST method to submit data to backend.

#### `studentexpenses.html`
- Student dashboard to view personal mess bills and attendance.
- Conditional rendering for months and records.

---

### 2. ⚙️ Backend – Flask App

- Built using **Python Flask Framework**.
- `@app.route` decorators used to handle different views and actions.
- Session-based login for secure access.
- Communicates with **MySQL** database using `pymysql`.
- Handles form data dynamically (submit, retrieve, and display).

---

### 3. 🗃️ SQL Database – `student_expense_db1.sql`

Creates and manages the following tables:
- `student` – Student details.
- `admin` – Admin credentials.
- `expense` – Total mess expenses by month.
- `attendance` – Student attendance data.
- `student_expense` – Monthly calculated expenses per student.

Includes:
- Initial data population.
- Foreign key relationships.

---

## 💡 Key Technologies

| Layer      | Technologies Used                |
|------------|----------------------------------|
| Frontend   | HTML5, CSS3, JavaScript, Bootstrap |
| Backend    | Python (Flask)                   |
| Database   | MySQL                            |
| Tools      | Google Fonts, VS Code, Postman   |
| Hosting    | Localhost (XAMPP/WAMP), or Cloud Platforms |

---

## 👨‍💼 Admin Features

- **Secure Login** to backend.
- **Manage Students**: Add, update, delete student details.
- **Record Monthly Expenses**.
- **Input Student Attendance**.
- **Auto-Calculate Bills** based on attendance.
- **Admin Dashboard**: View statistics and control features.

---

## 🧑‍🎓 Student Features

- **Login** using ID and Phone Number.
- **View Mess Bill**: Monthly history.
- **Check Attendance**: See monthly attendance records.
- **Profile View** on dashboard.

---

## 🗃️ Database Tables

| Table Name        | Description                                 |
|-------------------|---------------------------------------------|
| `student`         | Stores student ID, name, branch, phone      |
| `admin`           | Stores admin login credentials              |
| `expense`         | Monthly total mess expenses                 |
| `attendance`      | Student attendance data per month           |
| `student_expense` | Computed student-wise monthly expenses      |

---

## 📸 Output Flow (UI Screens)

- **Home Page**: Navigation to Admin and Student Login  
![Screenshot 2025-05-26 190132](https://github.com/user-attachments/assets/59881f4b-25f4-4c9e-b256-5b125a7c65c9)

- **Admin Login**: Username/password authentication → Dashboard  
![Screenshot 2025-05-26 190309](https://github.com/user-attachments/assets/f203b2b0-0a64-433a-be5d-f7a8223b11f4)

- **Student Registration**: Inputs → Stored in DB → Success message  
![Screenshot 2025-05-26 192739](https://github.com/user-attachments/assets/04279be2-37f4-4346-a0dd-98b93a09a337)

- **Student Login**: ID and phone verification → Dashboard  
![Screenshot 2025-05-26 193020](https://github.com/user-attachments/assets/4c4a35e8-9bc0-48bd-bcef-bd031f74e895)

- **Admin Dashboard**: Add expense, attendance, view bills 
![Screenshot 2025-05-26 193216](https://github.com/user-attachments/assets/ad1aae1f-4da7-4397-9431-72d37203e101)
 
- **Attendance**: 
![Screenshot 2025-05-26 193400](https://github.com/user-attachments/assets/18a3b1ae-aaa2-4fe0-b231-578bcd1aa6f6)

- **Calculate Monthly Bill**:
![Screenshot 2025-05-26 193532](https://github.com/user-attachments/assets/5011eb5e-3eda-4290-9fc6-5504ae333ee3)

---

## 🔬 Further Research & Enhancements

### 🔐 Security Improvements
- Use password hashing
- Secure session handling
- Input validation (client + server)
- JWT for REST APIs
- HTTPS support

### 🚀 Features to Add
- Analytics in Admin Dashboard (charts, tables)
- Calendar-based attendance marking
- Payment receipt tracking
- Email/SMS notifications
- Mobile app integration

### 🎨 UI/UX Enhancements
- Modal forms and alerts
- Responsive layout using Flexbox/Grid
- Paginated and sortable tables
- Dark/Light mode toggle

### ☁️ Deployment Plans
- Docker container for uniform setup
- Deploy to Heroku, AWS, or GCP
- Setup CI/CD pipeline
- SSL certificate & custom domain
- SMTP integration for notifications

### 📊 Analytics Module
- Graphs for monthly student expenses
- Attendance trends
- Defaulters list
- Export reports (Excel, PDF)

### 💻 Code Optimization
- Modular Flask app using Blueprints
- ORM using SQLAlchemy
- Unit tests for key functionalities

### 📈 Scalability
- Multi-hostel/campus support
- Role-based access (SuperAdmin, Warden, Student)
- Load balancing & cloud-based DB

---

## 🔗 How to Run

1. Clone the repository
2. Import `student_expense_db1.sql` into MySQL
3. Run `app.py` with Flask:
   ```bash
   flask run
