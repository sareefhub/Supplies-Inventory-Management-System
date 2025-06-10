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

# วิธีการรันระบบ Supplies Inventory Management บน Localhost

## 📋 สิ่งที่ต้องติดตั้งก่อน (Prerequisites)

### 1. ติดตั้ง XAMPP หรือ WAMP
**สำหรับ Windows:**
- ดาวน์โหลด XAMPP จาก: https://www.apachefriends.org/download.html
- รันไฟล์ติดตั้งและเลือก Apache, MySQL, PHP, phpMyAdmin
- เปิด XAMPP Control Panel และเริ่ม Apache และ MySQL

**สำหรับ Mac:**
- ติดตั้ง MAMP หรือ XAMPP สำหรับ Mac
- หรือใช้ Homebrew: `brew install php mysql`

**สำหรับ Linux (Ubuntu/Debian):**
```bash
sudo apt update
sudo apt install apache2 mysql-server php php-mysql php-mbstring php-zip php-gd php-json php-curl
```

### 2. ติดตั้ง Node.js และ NPM
- ดาวน์โหลดจาก: https://nodejs.org/
- ตรวจสอบ: `node --version` และ `npm --version`

## 🚀 ขั้นตอนการติดตั้งระบบ

### ขั้นตอนที่ 1: Clone Repository

```bash
# Clone โปรเจ็กต์
git clone https://github.com/ProjectDevTeams/Supplies-Inventory-Management-System.git .
# หรือหากไม่มี git ให้ดาวน์โหลด ZIP และแตกไฟล์
```

```bash
# สร้างโฟลเดอร์สำหรับโปรเจ็กต์แล้วลากไฟล์ในโฟลเดอร์ backend มาใส่
mkdir C:\xampp\htdocs\backend
cd C:\xampp\htdocs\backend
```

### ขั้นตอนที่ 2: ตั้งค่าฐานข้อมูล

#### 2.1 เปิด phpMyAdmin
- เปิดเบราว์เซอร์ไปที่: http://localhost/phpmyadmin
- Login ด้วย username: `root` (password: ปล่าว หรือตามที่ตั้งไว้)

#### 2.2 สร้างฐานข้อมูล
```sql
-- ใน phpMyAdmin ไปที่แท็บ SQL และรันคำสั่งนี้
CREATE DATABASE supplies_inventory CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```

#### 2.3 Import ข้อมูล (หากมีไฟล์ SQL)
```bash
# หากมีไฟล์ database/schema.sql
mysql -u root -p supplies_inventory < database/schema.sql

# หรือใช้ phpMyAdmin Import ไฟล์ SQL โดยการลากไฟล์ supplies_inventory.sql มาใส่ใน http://localhost/phpmyadmin
```

#### ใช้ Apache (XAMPP) ในการรัน Server
1. วางโปรเจ็กต์ใน `C:\xampp\htdocs\backend`
2. เปิดเบราว์เซอร์ไปที่: http://localhost/backend

## 🌐 หน้าเว็บ Client

```bash
# เข้าโฟลเดอร์
cd client
```

```bash
# ดาวน์โหลดแพ็กเกจ
npm install
```

```bash
# รันโปรแกรม
npm start
```

```bash
# เข้าบราวเซอร์
npm start
```

- เปิดเบราว์เซอร์ไปที่: http://localhost:3000

## 🎯 เคล็ดลับสำหรับการพัฒนา

1. **ใช้ Environment Variables**: แยกข้อมูลการตั้งค่าออกจากโค้ด
2. **Backup Database**: สำรองฐานข้อมูลก่อนทำการเปลี่ยนแปลง
3. **Version Control**: ใช้ Git ในการติดตามการเปลี่ยนแปลง
4. **Testing**: ทดสอบฟีเจอร์ใหม่ในสภาพแวดล้อมพัฒนาก่อน

## 📞 การขอความช่วยเหลือ

หากยังมีปัญหา ลองตรวจสอบ:
1. **Error Logs**: ดูใน storage/logs/ หรือ Console
2. **PHP Version**: ตรวจสอบว่าใช้เวอร์ชันที่รองรับ
3. **Dependencies**: ตรวจสอบว่าติดตั้งครบถ้วน
4. **Permissions**: ตรวจสอบสิทธิ์การเข้าถึงไฟล์

**Happy Coding! 🚀**
