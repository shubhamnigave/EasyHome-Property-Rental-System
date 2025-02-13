🏡 Property Rental System
📌 Overview
The Property Rental System is a full-stack web application designed to streamline property rentals. It allows landlords to list properties, manage bookings, and handle payments, while tenants can search, book, and review properties. The system supports role-based access control for Landlords, Tenants, and Admins.

🚀 Features
✅ User Authentication (JWT) – Secure login and signup with role-based access (Tenant, Landlord, Admin).
✅ Property Management – Landlords can add, update, and delete property listings.
✅ Search & Filter – Tenants can search properties based on location, price, and amenities.
✅ Bookings & Payments – Tenants can book properties and pay online using Stripe.
✅ Reviews & Ratings – Tenants can provide feedback and rate properties.
✅ Admin Panel – Manage users, properties, and transactions with administrative privileges.
🏗️ Tech Stack
🔹 Backend:
Spring Boot – REST APIs, JWT Security
Spring Security – Authentication & Authorization
Hibernate + MySQL – Database Management
Docker – Containerized Deployment
🔹 Frontend:
React.js – User Interface
Redux – State Management
Tailwind CSS – Styling
Axios – API Requests
🔹 Other Tools:
Stripe API – Payment Gateway Integration
Swagger – API Documentation
Docker & Docker Compose – Deployment
GitHub Actions – CI/CD Pipeline
🎯 Database Schema
Users: id, name, email, password, role
Properties: id, title, description, address, rent, landlord_id
Bookings: id, tenant_id, property_id, start_date, end_date, payment_status
Reviews: id, user_id, property_id, rating, comments, created_at
Payments: id, booking_id, amount, status, created_at
