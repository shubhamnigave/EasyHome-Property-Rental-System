🏡 Property Rental System
Property Rental System

📌 Overview
The Property Rental System is a full-stack web application designed to streamline property rentals. It allows landlords to list properties, manage bookings, and handle payments, while tenants can search, book, and review properties. The system supports role-based access control for Landlords, Tenants, and Admins.

🚀 Features
✅ User Authentication (JWT) – Secure login/signup with role-based access (Tenant, Landlord, Admin).
✅ Property Management – Landlords can add, update, and delete properties.
✅ Search & Filter – Tenants can search properties based on location, price, and amenities.
✅ Bookings & Payments – Tenants can book properties and pay online via Stripe.
✅ Reviews & Ratings – Tenants can leave feedback on properties.
✅ Admin Panel – Manage users, properties, and transactions.

🏗️ Tech Stack
🔹 Backend:
Spring Boot (REST APIs, JWT Security)
Spring Security (Authentication & Authorization)
Hibernate + MySQL (Database Management)
Docker (Containerized Deployment)
🔹 Frontend:
React.js (User Interface)
Redux (State Management)
Tailwind CSS (Styling)
Axios (API Requests)
🔹 Other Tools:
Stripe API (Payment Gateway)
Swagger (API Documentation)
Docker & Docker Compose (Deployment)
GitHub Actions (CI/CD)
🎯 Database Schema
Users (id, name, email, password, role)
Properties (id, title, description, address, rent, landlord_id)
Bookings (id, tenant_id, property_id, start_date, end_date, payment_status)
Reviews (id, user_id, property_id, rating, comments, created_at)
Payments (id, booking_id, amount, status, created_at)
📷 Screenshots
Homepage	Property Details	Booking Page
Home	Details	Booking
🛠️ Installation & Setup
🔧 Prerequisites
Install Java 17+, Node.js, MySQL, Docker
🔹 Backend Setup
# Clone the repository
git clone https://github.com/your-username/property-rental-system.git
cd property-rental-system/backend

# Build and Run Spring Boot App
docker-compose up -d
🔹 Frontend Setup
cd ../frontend
npm install
npm start
🌍 Deployment
Docker (Local Setup)
docker-compose up -d
Deploy to Remote Server (Ubuntu)
scp -r ./property-rental-system user@server-ip:~/
ssh user@server-ip
cd property-rental-system
docker-compose up -d
📜 API Documentation
API Docs are available via Swagger UI:

http://localhost:8081/swagger-ui/index.html
