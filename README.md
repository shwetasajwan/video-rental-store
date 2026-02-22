# 🎬 Video Rental Store Management System

A database-driven desktop application that simulates the operations of a traditional video rental store.
This system manages customers, employees, inventory (movies, VCRs, video cameras), rental transactions, and payment tracking using a structured relational database.
Built using Python (Tkinter) for the GUI and MySQL for backend database management.

## 🔎 Project Overview

The application replicates a real-world rental store workflow:
- Customers browse and rent media items
- Employees manage transactions
- Payments are recorded and tracked
- Due dates and return dates are monitored
- Database ensures data integrity and consistency

The project focuses on database schema design, relational integrity, and transaction management.

## 🧠 System Architecture
1. User Management
- Users: user_id, username, password, email
- Customers: customer_id, name, email, phone_number
- Employees: employee_id, name, position

2. Inventory Management
- Movies: movie_id, name, director, producer, genre/type, charge_per_day, quantity

3. VCR
- vcr_id
- brand_name
- type
- made_by
- charge
- quantity

4. Video Camera
- video_camera_id
- brand_name
- made_by
- charge
- quantity

5. Transaction Management
- Separate transaction tables ensure structured rental tracking: Movie_Transactions, VCR_Transactions, VCamera_Transactions
- Each transaction stores: transaction_id, item_id, customer_id, employee_id, amount_paid, due_date, return_date, rental_type

6. Payment System
- Tracks: Payment method, Payment amount, Transaction date, Associated transaction ID

7. Categories
- Defines classifications for: Movies, VCR, Video Cameras

## 🛠️ Tech Stack
# Layer and	                      Technology
  GUI:	                        Python (Tkinter), 
  Backend:                    MySQL,
  Database Integration:	      mysql.connector,
  Validation:	                Regular Expressions (re)

## 🚀 Key Functionalities

- Add / Update / Delete customers 
- Inventory management
- Rental transaction processing
- Late return tracking
- Payment recording
- Data validation using RegEx
- Relational database constraints

## 📌 What This Project Demonstrates

- Relational database schema design
- Normalization principles
- Foreign key constraints
- Transaction handling
- Python–MySQL integration
- GUI development using Tkinter

## 🎯 Future Improvements

- Single unified transaction table (normalized schema)
- Fine calculation automation
- Admin dashboard analytics
- Role-based authentication
- REST API migration
