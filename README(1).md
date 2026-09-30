# Web-Based Hotel Booking System for Galilee Hotel

A web-based hotel booking system for **Galilee Hotel** that replaces the traditional manual booking process with a digital platform where guests can browse rooms, check availability, make reservations, manage their bookings, and view hotel offers.

The system is built to provide a simple, organized, and convenient booking experience for guests while giving hotel staff an administrative system for managing rooms, reservations, promotions, amenities, and users.

---

## Key Features

### Customer Room Browsing
- View available room types and room details
- View room descriptions, capacity, bed configuration, amenities, prices, and room images
- Check room availability based on selected check-in and check-out dates

### Hotel Booking
- Select check-in and check-out dates
- Choose number of guests and rooms
- Calculate room cost and additional guest fees
- Submit a reservation as a guest or logged-in user
- Receive a unique reservation code

### Reservation Management
- View current and previous reservations
- Search for a reservation using reservation code and email
- View reservation details and status
- Cancel eligible reservations

### User Authentication
- Register a customer account
- Login using email and password
- Google login support
- Token-based authentication for protected features

### Hotel Offers and Promotions
- Display active promotions on the customer website
- Manage promotional banners and links through Django Admin
- Control promotion order and visibility

### Django Admin
- Manage reservations
- Manage room types and individual rooms
- Manage room images
- Manage amenities
- Manage promotions
- Manage users and user profiles
- Use Django's built-in Groups and Tokens management
- View booking status information from the customized admin dashboard

---

## Project Members

| Name | Role |
|---|---|
| De Leon, Kurt Christian T. | Project Manager |
| Santiago, Neil Ryann T. | UI/UX Designer |
| Tadeo, Brent Garreth G. | UI/UX Designer |
| Sumagaysay, John Michael O. | Frontend Developer / Researcher |
| Dy, Jay Brian M. | Frontend Developer |
| Santiago, Carl Emmanuel M. | Documentation / Tester |

---

## Technologies Used

### Frontend
- **HTML5** - page structure
- **CSS3** - styling and layout
- **JavaScript** - interactivity and application logic
- **React** - frontend user interface
- **Vite** - frontend development and build tool
- **Tailwind CSS** - responsive UI styling
- **Axios** - API requests
- **React Router** - page navigation
- **Lucide React** - interface icons

### Backend
- **Python** - backend programming language
- **Django** - web framework and admin system
- **Django REST Framework** - REST API
- **django-cors-headers** - frontend/backend cross-origin communication
- **Django REST Framework Token Authentication** - API authentication
- **Pillow** - image handling

### Database
- **SQLite** - default local development database
- **PostgreSQL** - supported for production deployment

### Deployment
- **Vercel** - frontend deployment
- **Render** - backend deployment

---

## Project Structure

```text
galilee-hotel-booking-main/
├── backend/
│   ├── bookings/
│   ├── config/
│   ├── templates/
│   ├── manage.py
│   └── requirements.txt
│
└── frontend/
    ├── public/
    ├── src/
    ├── package.json
    └── vite.config.js
```

---

## Live Deployment

- **Frontend:** https://galilee-hotel-booking.vercel.app/
- **Django Admin:** https://galilee-hotel-booking.onrender.com/admin/

---

## Local Development

### Frontend

```bash
cd frontend
npm install
npm run dev
```

The frontend will normally run at:

```text
http://localhost:5173/
```

### Backend

```bash
cd backend
python -m venv venv
venv\Scripts\activate
python -m pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

The Django backend will normally run at:

```text
http://localhost:8000/
```

The Django Admin is available at: 

```text
http://localhost:8000/admin/
```

The frontend uses `VITE_API_BASE_URL` to connect to the Django REST API. For local development, the default API base URL is:

```text
http://localhost:8000/api
```

---

## Purpose of the System

The main purpose of the Galilee Hotel Booking System is to make the hotel reservation process easier for customers and more manageable for hotel staff. The frontend provides the customer booking experience, while Django provides the API, database access, authentication, and administrative management system.
