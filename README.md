# E-Trade Web Application

## Overview
https://oms.egitdns.net/

A robust and scalable web application built with **Angular**, **SignalR**, and **.NET Core**, designed for seamless electronic trading (E-trade). It supports real-time data feeds, advanced stock market analysis, and secure order placement, with separate experiences tailored for **brokers** and **individual clients**.

The application also features powerful modules for **portfolio management**, **credit and margin control**, **IPO trading**, and **fund management**, with advanced capabilities for **bulk order handling** and dynamic UI configurations.

---

## Features

### 🚪 Dual Version Support
- **Broker View**: Comprehensive tools for managing multiple clients, bulk trading, credit control, and high-volume order management.
- **Client View**: Streamlined interface tailored for individual traders, focusing on portfolio performance, quick trading, and analytics.
![image](https://github.com/user-attachments/assets/adbe7c52-d5fa-433b-b293-a86b13ff28fe)
---

### 🪟 Docking System

An advanced window docking system that allows users to:
- Open multiple live data windows simultaneously.
- Maintain synchronized interactions — a selection in one window updates data across all others.
- Freely resize, pin, tab, or reposition windows.
- Build and save fully customized layouts for trading setups.

https://github.com/user-attachments/assets/e7166687-0da3-45b3-9cee-bd7d2ab86d55
 
-Pinning

https://github.com/user-attachments/assets/bae83bcd-14d5-4060-90d7-411bbb87da49

---

### 💾 Layout Management

- Save and load multiple custom window layouts.
- Preserve state, size, position, and data context of all open windows.
- Quickly switch between different workflow setups.
  
https://github.com/user-attachments/assets/2e5054b4-d19b-4554-980a-5bcd09fa05ec

---

### ⚡ Flashing Cells (Live Data Highlighting)
 **As shown in the dokcing video**
- Efficient SignalR backend hub to deliver real-time stock updates.
- Handles updates for over **300 stocks**.
- Uses a smart difference checking algorithm to detect which stocks were updated.
- Only flashes updated cells with red (decrease) or green (increase) indicators.
- Maintains data integrity and high-speed performance with zero delay.

---

### 🔐 Authentication & Token Management

- Implements secure JWT-based authentication.
- Supports **refresh token integration**:
  - Keeps users logged in as long as they remain active.
  - Prevents token expiration from disrupting user sessions.
  - Maintains authentication integrity without unnecessary re-authentication.

---

### 📊 Stock Analysis Module

- Full stack support (Backend & Frontend).
- Access to current and historical data for every stock.
- Interactive and zoomable graphs.
- Visual analysis tools for trends, volume, and price fluctuations.
  
![Stock analysis](https://github.com/user-attachments/assets/6a4d5ad6-990a-47cc-8bc6-4f8211fc1921)

---

### 🚀 IPO Module

- Full stack support (Backend & Frontend).
- Visual representation of IPO offerings.
- Dynamic order fees and **Price-to-Earnings (P/E)** ratio calculations.
- Real-time updates and validations during IPO bidding.
  
![image](https://github.com/user-attachments/assets/2c1466c1-c749-4b34-af63-449fe219c736)

---

### 💼 Fund Management Module

- Full stack support (Backend & Frontend).
- Handles various fund types (mutual, index, ETFs).
- Live cash-to-stock calculations.
- Dynamic fee structure integrated with each transaction.
  
https://github.com/user-attachments/assets/5a6c0eb4-e8f7-4d3f-a1ac-9b3c0fc35a01

---

### 📦 Bulk Order Processing

- Store and manage pending orders in a local **basket**.
- Submit multiple orders simultaneously to the market.
- Built-in safety checks to prevent budget overruns.
- Validates purchase power for each client before executing the next order.
- Integrates with FIX server to track and update the status of every order.
  
![image](https://github.com/user-attachments/assets/b0cf56a3-8521-4eb5-aa8b-0920673b0c4d)

---

### 🛒 Dynamic Buy/Sell Ticket

- Interactive trade ticket for buying and selling.
- Dynamically calculates order fees based on:
  - Current market conditions.
  - Client purchase power.
- Ensures accurate trading cost before confirmation.
  
https://github.com/user-attachments/assets/ec06a226-6c38-4194-ae98-4e1fdb37b33f

---

### 🌐 Multi-language Support

- Supports **two languages** with dynamic localization.
- Automatically adapts content based on user language settings.
  
https://github.com/user-attachments/assets/88b72cb3-720a-4f3a-8553-8ab667826d34

---

### 🌙 Theme Support

- Toggle between **Light** and **Dark** themes.
- Consistent and responsive styling for all components.
  
https://github.com/user-attachments/assets/20ff76d2-55c7-4efb-bfb3-93d1a4bdd0fd

---

## Tech Stack

- **Frontend**: Angular, RxJS, SignalR Client
- **Backend**: .NET Core, SignalR, REST API, FIX protocol integration
- **Authentication**: JWT + Refresh Tokens
- **Realtime Engine**: SignalR Hubs for live feeds and UI updates

