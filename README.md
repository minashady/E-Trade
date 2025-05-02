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

---

### 🪟 Docking System

An advanced window docking system that allows users to:
- Open multiple live data windows simultaneously.
- Maintain synchronized interactions — a selection in one window updates data across all others.
- Freely resize, pin, tab, or reposition windows.
- Build and save fully customized layouts for trading setups.

---

### 💾 Layout Management

- Save and load multiple custom window layouts.
- Preserve state, size, position, and data context of all open windows.
- Quickly switch between different workflow setups (e.g., IPO trading, live analysis, order monitoring).

---

### ⚡ Flashing Cells (Live Data Highlighting)

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

---

### 🚀 IPO Module

- Full stack support (Backend & Frontend).
- Visual representation of IPO offerings.
- Dynamic order fees and **Price-to-Earnings (P/E)** ratio calculations.
- Real-time updates and validations during IPO bidding.

---

### 💼 Fund Management Module

- Full stack support (Backend & Frontend).
- Handles various fund types (mutual, index, ETFs).
- Live cash-to-stock calculations.
- Dynamic fee structure integrated with each transaction.

---

### 📦 Bulk Order Processing

- Store and manage pending orders in a local **basket**.
- Submit multiple orders simultaneously to the market.
- Built-in safety checks to prevent budget overruns.
- Validates purchase power for each client before executing the next order.
- Integrates with FIX server to track and update the status of every order.

---

### 🛒 Dynamic Buy/Sell Ticket

- Interactive trade ticket for buying and selling.
- Dynamically calculates order fees based on:
  - Current market conditions.
  - Client purchase power.
- Ensures accurate trading cost before confirmation.

---

### 🌐 Multi-language Support

- Supports **two languages** with dynamic localization.
- Automatically adapts content based on user language settings.

---

### 🌙 Theme Support

- Toggle between **Light** and **Dark** themes.
- Consistent and responsive styling for all components.

---

## Tech Stack

- **Frontend**: Angular, RxJS, SignalR Client
- **Backend**: .NET Core, SignalR, REST API, FIX protocol integration
- **Authentication**: JWT + Refresh Tokens
- **Realtime Engine**: SignalR Hubs for live feeds and UI updates

