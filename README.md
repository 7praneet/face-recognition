# Face Recognition Attendance System

A robust system designed to authenticate individuals and record attendance using **facial recognition technology** powered by deep learning. This project simplifies attendance tracking for classrooms, workplaces, or events.

## 📋 Features

- Role-based access for **administrators** and **lecturers**
- Manage courses, units, venues, and attendance records through an intuitive interface
- Capture and store multiple images for accurate identification
- Ideal for college projects

## Project Structure

```plaintext
Face-Recognition-Attendance-System/
├── database/
│   ├── attendance-db.sql         # SQL file to set up the database
│   └── database_connection.php   # Database connection script
├── models/
│   └── face-api-models.js        # JavaScript models for Face API
├── resources/
│   ├── assets/
│   │   ├── css/                  # CSS files
│   │   └── javascript/           # JavaScript files
│   ├── images/                   # Images directory
│   ├── labels/                   # Stored images of registered students
│   ├── lib/
│   │   └── global-functions.php  # Global PHP functions
│   ├── pages/
│   │   ├── admin/                # Admin-specific pages
│   │   ├── lecturer/             # Lecturer-specific pages
│   │   └── login.php             # Login page
├── index.php                     # Main entry point for all pages
├── .htaccess                     # Redirect rules
└── README.md                     # Project documentation
```

## 🚀 Setup Procedure

Follow these steps to set up and run the project:

### 1. Clone or Download the Repository

Clone the repository using Git:
```bash
git clone https://github.com/francis-njenga/Face-Recognition-Attendance-System.git
```
Alternatively, download the ZIP file.

### 2. Place the Project in the Server Directory

If you're using XAMPP, place the project folder inside the `htdocs` directory:
```plaintext
xampp/htdocs/Face-Recognition-Attendance-System
```
Use a simple folder name, as it will be part of the URL (e.g., attendance-system).

### 3. Start XAMPP
- Open the XAMPP Control Panel
- Start the **Apache** and **MySQL** services

### 4. Set Up the Database
1. Visit **phpMyAdmin**
2. Create a new database
   - Recommended name: `attendance_db` (You can choose any name, but ensure it matches the configuration in your project files)
3. Import the SQL file:
   - Locate the `attendance-db.sql` file in the `database/` folder of the project
   - Import it into the newly created database

### 5. Launch the Application

Visit the application in your browser:
```plaintext
http://localhost/{your-project-folder-name}
```

## 🧑‍💻 User Guide

### 1. Administrator Access
Login credentials:
- **Email**: `admin@gmail.com`
- **Password**: `@admin_`

Administrator capabilities:
- Add students
- Manage courses, units, and venues

⚠️ **Important Notes**:
- Add at least **two students** and capture **five clear images** for each
- Poor image quality will affect recognition accuracy
- You can retake any image by clicking on it

### 2. Lecturer Access
- Create a lecturer account via the admin panel or use pre-existing credentials

Default lecturer credentials:
- **Email**: `mark@gmail.com`
- **Password**: `@mark_`

*Note: Select lecture user type to login as lecturer. If you have issues using these credentials, create your lecturer account through the admin panel.*

Lecturer capabilities:
- Select course, unit, and venue on the home page
- Launch **Face Recognition** feature to begin attendance
- Export attendance to **Excel** sheets
- Access additional management features in the lecture panel
