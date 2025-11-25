# 💰 GeM Price Comparison Website

A web application to compare product prices on the Government e-Marketplace (GeM) with other e-marketplaces like Amazon, Flipkart, etc. The goal is to help buyers make informed purchasing decisions by tracking and analyzing price changes over time.

## 📦 Features

- 🔐 **User Authentication** (Register/Login/Password Reset)
- 📊 **Product Price Comparison** (GeM vs other e-marketplaces)
- ⏱️ **Price History Tracking** with Graphs
- 📬 **Email & SMS Alerts** for Price Drops
- 📱 **Mobile-Friendly Dashboard** for Users
- ⚙️ **Admin Panel** to Manage Products
- 💾 **Database Integration** for Storing Prices & User Data
- 💳 **Razorpay Integration** for Payments (and PhonePe QR Support)
- 📨 **Contact Form** with Optional Email Notification

## 🗂️ Project Structure

```
gem_price_comparison_website/
│
├── gem/                         # Main project folder (frontend + PHP backend)
│   ├── login/                   # Login and registration pages
│   ├── compare/                 # Product comparison pages
│   ├── dashboard/               # User dashboard with price tracking
│   ├── admin/                   # Admin functionality to manage products
│   ├── includes/                # PHP scripts for DB connection and utilities
│   └── assets/                  # CSS, JS, images
│
├── payment/                     # Razorpay & PhonePe payment integrations
│
├── database.sql                 # Database schema
├── README.md                    # Project documentation (this file)
└── .env                         # Environment variables (not tracked in Git)
```

## ⚙️ Tech Stack

- **Frontend**: HTML5, Tailwind CSS, JavaScript
- **Backend**: PHP
- **Database**: MySQL
- **Payment Gateway**: Razorpay, PhonePe QR
- **Alerts**: SMTP for email, Twilio (or similar) for SMS

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Alokkumarlpu/Gem_price_comparison_website.git
cd Gem_price_comparison_website
```

### 2. Setup Database

- Import the `database.sql` file into your MySQL server
- Update DB credentials in `includes/db.php`

### 3. Configure Environment Variables

Create a `.env` file (if required) for sensitive keys like:

```env
DB_HOST=localhost
DB_USER=root
DB_PASS=yourpassword
DB_NAME=gem_db

RAZORPAY_KEY=your_key
RAZORPAY_SECRET=your_secret

SMTP_USER=your_email
SMTP_PASS=your_email_password
```

### 4. Run Locally

Use XAMPP or similar to host the project locally and access via:

```
http://localhost/gem_price-comparison/
```






