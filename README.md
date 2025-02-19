# Bike Rental Portal

## Overview

The **Bike Rental Portal** is a web application that allows users to rent bikes online. It provides role-based dashboards for customers and bike rental companies, enabling seamless booking, management, and tracking of rentals. The system is built using **Flask** (backend), **MongoDB** (database), and **HTML, CSS, JavaScript** (frontend).

## Features

### **For Customers:**

- User registration & login
- View available bikes
- Book a bike for rental
- Track ongoing and completed bookings
- Profile management

### **For Companies:**

- Register & login
- Add, update, and remove bike details
- View completed bookings
- Track rented bikes

### **Admin Panel:**

- Manage users and roles
- Monitor system performance
- View analytics and reports

## Technology Stack

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python (Flask)
- **Database**: MongoDB
- **Authentication**: Flask-Login, bcrypt
- **Deployment**: Docker, Vercel (Frontend), AWS/GCP (Backend & DB)

## Project Structure

```
/bike-rental-portal
│── /templates  # HTML files
│── /static     # CSS, JavaScript, images
│── /routes     # Flask routes
│── /models     # Database models
│── /config     # Configuration settings
│── /utils      # Helper functions
│── app.py      # Main Flask application
│── config.py   # Configuration settings
│── requirements.txt  # Python dependencies
│── Dockerfile  # Containerization
│── README.md   # Project documentation
```

## Installation & Setup

### **Prerequisites**

- Install Python (3.8+ recommended)
- Install MongoDB (local or Atlas for cloud hosting)
- Install Docker (for containerized deployment)

### **Steps to Run the Project**

1. **Clone the repository**
   ```sh
   git clone https://github.com/your-username/bike-rental-portal.git
   cd bike-rental-portal
   ```
2. **Create a virtual environment (Optional but recommended)**
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```
3. **Install dependencies**
   ```sh
   pip install -r requirements.txt
   ```
4. **Set up environment variables**
   - Create a `.env` file and add MongoDB URI & secret keys:
   ```
   MONGO_URI=your_mongodb_connection_string
   SECRET_KEY=your_secret_key
   ```
5. **Run the application**
   ```sh
   python app.py
   ```
6. **Open the app in your browser**
   ```
   http://127.0.0.1:5000
   ```

### **Run with Docker**

1. **Build and run the container**
   ```sh
   docker build -t bike-rental-portal .
   docker run -p 5000:5000 bike-rental-portal
   ```
2. **Access the application**
   ```
   http://localhost:5000
   ```

## API Endpoints

| Method | Endpoint           | Description          |
| ------ | ------------------ | -------------------- |
| GET    | /                  | Home page            |
| POST   | /register          | User registration    |
| POST   | /login             | User login           |
| GET    | /dashboard         | User dashboard       |
| GET    | /bikes             | View available bikes |
| POST   | /book-bike         | Book a bike          |
| GET    | /company-dashboard | Company dashboard    |
| POST   | /add-bike          | Add a new bike       |
| GET    | /admin-dashboard   | Admin panel          |

## Future Enhancements

- Payment gateway integration
- Ride tracking with Google Maps
- AI-based price optimization
- Mobile app version
- Enhanced reporting and analytics

## License

This project is open-source and available under the **MIT License**.

---

🚀 Developed by **Narendra**
