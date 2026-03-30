# 🩸 Blood Donation & Inventory Management System

## Overview

A web-based system to manage blood donation, inventory tracking, issuing, and analytics using a real-world dataset. It simulates how a blood bank operates, focusing on stock management, expiry tracking, and donor records.

## Key Features

### 1. Dashboard

* Real-time overview of:

  * Total units
  * Available units
  * Expiring units
  * Total donors
* Blood group-wise stock visualization
* Usage distribution (Available / Used / Expired)
* Recent donor activity

### 2. Donor Management

* View all donor records
* Search by Donor ID
* Filter by blood group
* Displays complete donor details:

  * Age, gender, blood group
  * Hemoglobin, weight, BP
  * Donation history

### 3. Blood Collection

* Add new donation records
* Auto-calculates expiry (35 days)
* Validates required inputs
* Maintains collection log

### 4. Inventory Management

* Tracks all blood units
* Status classification:

  * Available
  * Used
  * Expired
* Filter by blood group and status
* Real-time stock updates

### 5. Blood Issue System

* Process hospital/patient requests
* FIFO (First In First Out) allocation
* Stock validation before issuing
* Maintains issue logs

### 6. Expiry Alerts

* Highlights units:

  * Critical: 1–3 days left
  * Warning: 4–7 days left
* Prevents wastage through early alerts
* Full expiry tracking table

### 7. Analytics

* Blood group distribution
* Inventory status charts
* Gender and age distribution
* Statistical summary:

  * Avg hemoglobin
  * Avg weight
  * Stock condition (Low / Critical / Sufficient)

## Tech Stack

* HTML5
* CSS3 (custom styling)
* JavaScript (Vanilla JS)
* Chart.js (for visualization)

## Dataset

* Source: Kaggle (Blood Bank Details)
* 50 real donor records
* Fields:

  * Donor ID
  * Age
  * Gender
  * Blood Group
  * Hemoglobin
  * Weight
  * Blood Pressure
  * Donation Date

## System Logic

### Expiry Calculation

* Blood expires after **35 days** from collection

### Stock Handling

* Each donor record = 1 blood unit
* Status auto-determined:

  * Expired (past date)
  * Available (valid)
  * Used (issued)

### Issuing Method

* FIFO (oldest available unit used first)

## How to Run

1. Copy the HTML file
2. Open in any modern browser
3. No backend required (runs fully on frontend)

## Limitations

* No database (data resets on refresh)
* No authentication
* Static dataset (except manual entries)

## Future Improvements

* Add backend (Node.js / Firebase / MySQL)
* User login system (Admin / Staff)
* Real-time database integration
* API integration with hospitals
* AI-based demand prediction
* SMS/email alerts for expiry

## Purpose

Built to demonstrate:

* Real-world problem solving
* Inventory management logic
* Data visualization
* Frontend system design

---

This is a simulation project, not a production-ready medical system.
