# appointment.queries
Database Schema
Users Table

user_id (Primary Key)
name
date_of_birth
email
phone
Clinics Table

clinic_id (Primary Key)
name
address
Doctors Table

doctor_id (Primary Key)
name
specialization
Doctor_Clinics Table

doctor_clinic_id (Primary Key)
doctor_id (Foreign Key)
clinic_id (Foreign Key)
Appointments Table

appointment_id (Primary Key)
user_id (Foreign Key)
doctor_clinic_id (Foreign Key)
appointment_time (DATETIME)
status (ENUM('Scheduled', 'Cancelled', 'Completed'))
created_at (DATETIME)
