![image](https://github.com/user-attachments/assets/043ebab5-df39-4f53-b0c1-e537e836ea28)

# Supplies Inventory Management System

A comprehensive inventory management system designed to help businesses efficiently track, manage, and control their supplies and inventory operations.

## 🌟 Overview

The Supplies Inventory Management System is a robust solution that enables businesses to maintain accurate inventory records, track stock movements, manage suppliers, and generate comprehensive reports. Whether you're running a small retail shop or managing warehouse operations, this system provides the tools you need to streamline your inventory processes.

## ✨ Features

### Core Functionality
- Inventory Tracking Real-time monitoring of stock levels, locations, and movements
- Product Management Add, edit, and categorize products with detailed specifications
- Supplier Management Maintain supplier information and track purchase history
- Stock Alerts Automated notifications for low stock, expiring items, and reorder points
- Barcode Support Generate and scan barcodes for efficient product identification

### Advanced Features
- Multi-location Support Track inventory across multiple warehouses or stores
- Purchase Order Management Create, approve, and track purchase orders
- Sales Order Processing Handle customer orders and track fulfillment
- Inventory Valuation Calculate inventory value using FIFO, LIFO, or weighted average methods
- Reporting & Analytics Generate detailed reports on inventory performance, trends, and forecasting

### User Management
- Role-based Access Control Different permission levels for administrators, managers, and staff
- User Activity Logging Track all system activities for audit purposes
- Secure Authentication Encrypted login system with session management

## 🛠️ Technology Stack

- Frontend HTML5, CSS3, JavaScript, Bootstrap
- Backend PHP 8.0+  Python 3.8+  Node.js (specify your choice)
- Database MySQL 8.0+  PostgreSQL
- Additional Libraries 
  - Chart.js for data visualization
  - DataTables for enhanced table functionality
  - PDF generation library for reports

## 📋 Prerequisites

Before you begin, ensure you have the following installed

- Web server (ApacheNginx)
- PHP 8.0+ (if using PHP backend) or Python 3.8+ (if using Python)
- MySQL 8.0+ or PostgreSQL
- Composer (for PHP dependencies) or pip (for Python dependencies)
- Node.js and npm (for frontend dependencies)

# How to Run Supplies Inventory Management System on Localhost

### 1. Install XAMPP or WAMP

**For Windows:**

-   Download XAMPP from: https://www.apachefriends.org/download.html
-   Run the installer and select Apache, MySQL, PHP, phpMyAdmin
-   Open XAMPP Control Panel and start Apache and MySQL

**For Mac:**

-   Install MAMP or XAMPP for Mac
-   Or use Homebrew: `brew install php mysql`

**For Linux (Ubuntu/Debian):**

```bash
sudo apt update
sudo apt install apache2 mysql-server php php-mysql php-mbstring php-zip php-gd php-json php-curl

```

### 2. Install Node.js and NPM

-   Download from: https://nodejs.org/
-   Verify installation: `node --version` and `npm --version`

## 🚀 System Installation Steps

### Step 1: Clone Repository

```bash
# Clone the project
git clone https://github.com/ProjectDevTeams/Supplies-Inventory-Management-System.git .
# Or if you don't have git, download ZIP and extract files

```

```bash
# Create folder for the project and move backend files
mkdir C:\xampp\htdocs\backend
cd C:\xampp\htdocs\backend

```

### Step 2: Database Setup

#### 2.1 Open phpMyAdmin

-   Open browser and go to: http://localhost/phpmyadmin
-   Login with username: `root` (password: empty or as configured)

#### 2.2 Create Database

```sql
-- In phpMyAdmin, go to SQL tab and run this command
CREATE DATABASE supplies_inventory CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;

```

#### 2.3 Import Data (if SQL file exists)

```bash
# If you have database/schema.sql file
mysql -u root -p supplies_inventory < database/schema.sql
# Or use phpMyAdmin Import feature by dragging supplies_inventory.sql file to http://localhost/phpmyadmin

```

#### Using Apache (XAMPP) to Run Server

1.  Place the project in `C:\xampp\htdocs\backend`
2.  Open browser and go to: http://localhost/backend

## 🌐 Client Web Application

```bash
# Navigate to folder
cd client

```

```bash
# Install packages
npm install

```

```bash
# Run the application
npm start

```

-   Open browser and go to: http://localhost:3000
