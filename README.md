## 👥 Project Contributors — Group OF Five

This project was collaboratively developed by **Group Five**.  
Each member actively contributed to the design, development, and completion of the project.

### 📌 Team Members

| Name               | ID        | GitHub Username |
|--------------------|-----------|-----------------|
| Abdurahman Kedir   | 0494/16   | [@abdikee](https://github.com/abdikee) |
| Kedeflah Nure      | 1724/16   | [@Aflah-Dev](https://github.com/Aflah-Dev) |
| Abdulhefiz Worko   | 0470/16   | [@abwa](https://github.com/abwa) |
| Mulu Beshada       | 2093/16   | [@mulu31](https://github.com/mulu31) |
| Ana Umer           | 0706/16   | [@ana-umer](https://github.com/ana-umer) |

---

> Built with teamwork, responsibility, and shared learning 🤝

Application is live on https://green-spider-729183.hostingersite.com/

# 🏥 PharmaPulsecy Management System

A comprehensive, **mobile-responsive** pharmacy management system built with PHP and MySQL. Designed for modern pharmacies with complete inventory management, point of sale, and administrative features.

![PHP](https://img.shields.io/badge/PHP-8.3+-777BB4?style=flat&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0+-4479A1?style=flat&logo=mysql&logoColor=white)
![Mobile](https://img.shields.io/badge/Mobile-Responsive-28a745?style=flat&logo=mobile&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-blue.svg)

## 🌟 Features

### 💊 **Core Pharmacy Management**

- **Inventory Management** - Complete stock tracking with FEFO (First Expired, First Out)
- **Point of Sale (POS)** - Professional transaction processing
- **Product Catalog** - Comprehensive product and category management
- **Supplier Management** - Track suppliers and purchase history
- **Expiry Monitoring** - Automated alerts for expiring medications

### 📱 **Mobile-First Design**

- **Fully Responsive** - Works perfectly on phones, tablets, and desktops
- **Touch-Optimized** - Large buttons and touch-friendly interface
- **Mobile Navigation** - Hamburger menu with smooth animations
- **Adaptive Tables** - Tables transform to card layout on mobile
- **Mobile Forms** - Optimized for mobile keyboards and input

### 👥 **User Management**

- **Role-Based Access** - Admin, Pharmacist, Cashier roles
- **Secure Authentication** - Password hashing and session management
- **Activity Logging** - Complete audit trail of user actions
- **Permission System** - Granular access control

### 📊 **Reporting & Analytics**

- **Sales Reports** - Daily, weekly, monthly sales analysis
- **Stock Reports** - Inventory levels and valuation
- **Expiry Reports** - Track expiring medications
- **Financial Reports** - Revenue and profit analysis

### 🔐 **Security Features**

- **CSRF Protection** - Cross-site request forgery prevention
- **XSS Prevention** - Input sanitization and output encoding
- **Session Security** - Secure session management with timeouts
- **SQL Injection Protection** - Prepared statements throughout

## 🚀 Quick Start

### Prerequisites

- PHP 8.0 or higher
- MySQL 8.0 or higher
- Web server (Apache/Nginx) or PHP built-in server

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/Aflah-Dev/PharmaPulse-Pharma.git
   cd PharmaPulse-Pharma
   ```

2. **Set up the database**

   ```bash
   # Create database
   mysql -u root -p -e "CREATE DATABASE pharmapulse CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;"

   # Import schema
   mysql -u root -p pharmapulse < schema.sql
   ```

3. **Configure environment**

   ```bash
   # Copy environment file
   cp .env.example .env

   # Edit database credentials
   nano .env
   ```

4. **Start the application**

   ```bash
   # Using PHP built-in server
   php -S localhost:8000

   # Or configure your web server to point to the project directory
   ```

5. **Access the application**
   - Open: green-spider-729183.hostingersite.com
   - Login with the admin account created during setup

## 📱 Mobile Experience

### Desktop View

- Full sidebar navigation
- Multi-column layouts
- Comprehensive data tables
- Advanced form layouts

### Mobile View

- Hamburger menu navigation
- Single-column responsive layout
- Card-style data presentation
- Touch-optimized forms and buttons

### Testing Mobile Responsiveness

- **Mobile Debug Page**: `/mobile-debug.php`
- **Mobile Test Page**: `/mobile-test.php`
- **POS Mobile Test**: `/mobile-pos-test.html`

## 🏗️ Architecture

### Directory Structure

```
📁 PharmaPulse-Pharma/
├── 📄 index.php                 # Main entry point
├── 📄 schema.sql               # Database structure
├── 📄 database_check.php       # System verification
├── 📁 assets/
│   ├── 📁 css/                 # Responsive stylesheets
│   ├── 📁 js/                  # Mobile-optimized JavaScript
│   └── 📁 images/              # Application assets
├── 📁 config/
│   └── 📄 database.php         # Database configuration
├── 📁 includes/
│   ├── 📄 auth.php             # Authentication functions
│   ├── 📄 security.php         # Security utilities
│   └── 📄 alerts.php           # Alert system
├── 📁 modules/
│   ├── 📁 auth/                # Login/logout system
│   ├── 📁 dashboard/           # Main dashboard
│   ├── 📁 sales/               # POS and sales history
│   ├── 📁 stock/               # Inventory management
│   ├── 📁 products/            # Product management
│   ├── 📁 reports/             # Reporting system
│   ├── 📁 suppliers/           # Supplier management
│   └── 📁 users/               # User management
└── 📁 templates/
    ├── 📄 header.php           # Common header
    ├── 📄 sidebar.php          # Navigation sidebar
    └── 📄 footer.php           # Common footer
```

### Database Schema

- **users** - User accounts and roles
- **products** - Product catalog
- **product_categories** - Product categorization
- **suppliers** - Supplier information
- **stock_batches** - Inventory with batch tracking
- **sales** - Transaction records
- **sale_items** - Transaction line items
- **stock_adjustments** - Inventory adjustments
- **activity_logs** - Audit trail

## 🛠️ Technology Stack

- **Backend**: PHP 8.3+ with PDO
- **Database**: MySQL 8.0+ with InnoDB
- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Custom CSS with CSS Grid and Flexbox
- **Icons**: Font Awesome 6.4.0
- **Security**: CSRF tokens, prepared statements, input sanitization

## 📊 Features Overview

### Point of Sale (POS)

- Real-time product search
- Shopping cart functionality
- Multiple payment methods (Cash, Card, Mobile Money)
- Automatic tax calculation
- Receipt generation
- FEFO batch allocation

### Dashboard

- Key performance indicators
- Recent sales overview
- Expiry alerts
- Low stock notifications
- Quick action buttons

### Inventory Management

- Product catalog with categories
- Batch tracking with expiry dates
- Stock level monitoring
- Automatic reorder alerts
- Stock adjustment tracking

### User Roles

- **Admin**: Full system access
- **Pharmacist**: Inventory and sales management
- **Cashier**: POS and basic inventory view

## 🔧 Configuration

### Environment Variables (.env)

```env
# Database Configuration
DB_HOST=127.0.0.1
DB_NAME=pharmapulse
DB_USER=root
DB_PASS=

# Application Settings
APP_ENV=production
APP_TIMEZONE=Africa/Addis_Ababa
SESSION_TIMEOUT=3600
```

### Default Users

- An initial **Administrator** account is created during setup — set its credentials in your own `.env`/seed step rather than using a shared default.

## 📱 Mobile Optimization

### Responsive Breakpoints

- **Desktop**: 1200px+
- **Laptop**: 1024px+
- **Tablet**: 768px+
- **Mobile**: 480px+
- **Small Mobile**: 360px+

### Mobile Features

- Touch-friendly buttons (44px minimum)
- Swipe-friendly tables
- Mobile keyboard optimization
- Hamburger menu navigation
- Card-style data layouts

## 🧪 Testing

### Manual Testing

```bash
# Database verification
php database_check.php

# Mobile responsiveness
# Open mobile-debug.php in browser
# Test different screen sizes
```

### Browser Testing

- Chrome (Desktop & Mobile)
- Safari (iOS & macOS)
- Firefox (Desktop & Mobile)
- Edge (Desktop & Mobile)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built for modern pharmacy management needs
- Designed with mobile-first approach
- Focused on user experience and security
- Ethiopian pharmacy regulations compliant

## 📞 Support

For support and questions:

- Create an issue on GitHub
- Check the documentation in `/docs`
- Review the mobile testing pages

---

**🏥 PharmaPulse Management System - Professional, Mobile-Responsive, Secure** 🚀
